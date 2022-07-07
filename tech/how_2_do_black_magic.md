### How to do black magic (blogging made hard af) [7/7/22]
First, you need to make 2 repositories:
- GitHub Pages (ex. greysoh.github.io)
- Pages Source (ex. blog-maybe)  
  
Then, you need to add 2 secrets in the pages source repo:
- GitHub Token (look it up am lazy), as TOKEN
- Your git email, as EMAIL  
  
Then, proceed to get your last little bit of sanity, and copy and paste all of this into `.github\workflows\build.yml`, in the pages source repo:
```yml
name: Build repo
on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-node@v3
        with:
          node-version: 18

      - name: Making input directory
        run: mkdir /tmp/stuff
        
      - name: Copying files
        run: cp -r . /tmp/stuff

      - name: Deleting files
        run: rm -rf * && rm -rf /tmp/stuff/.git*

      - name: Downloading blogging software...
        run: git clone https://github.com/greysoh/blog-gen.git

      - name: Installing blogging software...
        run: cd blog-gen && npm install

      - name: Running blogging software...
        run: cd blog-gen && cp -r /tmp/stuff in && npm start

      - name: Listing files (for debugging)
        run: cd blog-gen && ls out

      - name: Downloading blog...
        run: git clone https://github.com/user/github-pages.git pages
      
      - name: Deleting existing files...
        run: mv pages/CNAME . && rm -rf pages/* && mv CNAME pages/
      
      - name: Copying new files...
        run: cp -r blog-gen/out/* pages/
      
      - name: Setting config...
        shell: bash
        env: 
          EMAIL: ${{ secrets.EMAIL }}
          PASS: ${{ secrets.TOKEN }}
        run: git config --global user.name "user" && git config --global user.email "$EMAIL"
      
      - name: Commiting changes...
        run: cd pages && git add . && git commit -m "Sync changes"

      - name: Pushing changes...
        uses: cpina/github-action-push-to-another-repository@main
        env:
          API_TOKEN_GITHUB: ${{ secrets.TOKEN }}
        with:
          source-directory: 'pages'
          destination-github-username: 'user'
          destination-repository-name: 'github-pages'
          user-email: ${{ secrets.EMAIL }}
          target-branch: main
```
Replace `user`, with your username, and `github-pages`, with the github pages repository.  
  
Then, make a file named `template.html`, in the root of the pages source repo, and make something similar to this:
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Epic Site</title>
    </head>
    <body>
        Some markdown below:<br><br>
        <md></md>
    </body>
</html>
```
Remember that `<md></md>` is where the markdown gets inserted.  
  
Finally, make a test file, named `index.md`, at the root in the same repo, and put whatever markdown you want in there.  

Good luck I guess.
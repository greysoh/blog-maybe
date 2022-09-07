# The road to a (better) Window Server [9/6/22]
## Info
This article is not very technical, I just want to show off mostly. I'll make a more technical version once I get my WindowServer in a better shape.
## Intro
I've been working on my [operating system](https://eclipse.greysoh.xyz) ([source code](https://github.com/Eclipse-JS/eclipse)) for about 2 weeks now (after being rewritten from my old project, JSKernel, and I wanna share how I got to a basic window server from a bad OS I made.
## Nuking
I decided to nuke the old version 2 weeks ago, and make my own. I already had the basics down, such as processes (actually, that's the only thing I already had planned).  
  
I decided to go for the Microkernel architecture (nearly everything runs in userspace, except fetching the framebuffer, and running executables), which fit JS well and I thought it was simple.
## Planning
Everything I write in my code is planned (architecture wise) ahead of time. From the filesystem (took me 4 main revisions to get right, and 4 more on top of that to add security), to the shell.
## Kernel
The kernel is very simple. Just executes code and has a framebuffer. That's it.  
  
Oh, did I mention it has a JavaScript `require()` like system built in? (Not to be confused with `qb.require()` and `require()` in the code)  
  
Yeah, my code has Kernel extensions, for libraries. Nearly everything needs it. From the filesystem, to the security and eventually the Window Server.
## VFS
The filesystem is incredibly simple. I tried making something efficient but failed miserably. So, I decided to just push all the directories and files into one directory. (I don't know how I've lived this long without rm support :p)
## Security
Security was a tough one. I had made a users parser in userspace, which meant security had to be done in userspace, which was incredibly difficult.  
  
I added custom kernels per app in my code, which is only used in security, and is disabled after that. The security system just fetches the user info and if you have the right permissions, you can essentially be god (besides some features).
  
For example, you do not have access to `localStorage`, `document`, `self`, or others, and have to use abstraction layers to access the data.  
  
But, if you are root, you do not need abstraction layers, and can interface directly (abstractions are still encouraged, however).
  
After a night of hard work, I finally had support for security. But there was 1 small problem.
## Migration to [qbuild](https://github.com/Eclipse-JS/qbuild)
Code got long. And I mean LONG. For example:  
  
`(was) /repos/main/pkg.js`  
  
```js
216  default: {
217    input.stdout("ERR: No commands specified!\n\n");
218    help();
219    
220    break;
221  }
222 }
```
I caved in, and made a custom build system. Now, everything is split into small(ish) chunks. Not really much to talk about, except boring work.
## Misc stuff
I was thinking about copy.sh's v86 project, and DOOM, but decided that a: it may be out of my league yet, and b: it would probably work better if I implement my Window Server first.
## WindowServer
Alright, here goes.  
  
The Window Server has a simple architecture, and I'm only expecting it to be around ~400 lines of code, **MAX**. It has to run as root (because Security requires it to be able to register Kernel extensions, kinda like JS libraries).
  
I found out this wonderful feature (no, seriously!), in that you could have nested canvases, by using drawImage to draw it onto the screen.  
  
Immediately, I started work on the Window Server, and you could even see my [architecture plans](https://github.com/Eclipse-JS/eclipse/issues/4) (probably a bit different than what I implemented, as I didn't read it, oops!)  
  
It works exactly like stated (so far), so I really don't have anything to say, other then the fact that the canvas system works(!)
## Conclusion
I would appreciate some pull requests to fix the good amount of FIXME's and TODO's in the code. And the Window Server is almost ready for prime time.  
  
I still need to implement drawing on the top, moving windows, and keyboard and mouse handling.  
  
But other than that, happy Tuesday! (or whatever day it is, lol)
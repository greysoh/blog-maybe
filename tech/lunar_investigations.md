### Lunar Client Investigations [8/24/22]
I'll be adding to this when I dig more into the logs.  
  
I found these log messages, while developing my custom launcher:
```
[Client thread/INFO]: [LC Ichor] Disabling ReplayMod because there is no valid link.
[Client thread/INFO]: [LC Ichor] Disabling NEU because there is no valid link.
```
Could Replay Mod be in the source code still?  
  
Here's the full log incase you guys wanna investigate:
```
C:\Users\Greys\Documents\git\lcf2>lcf2
 ? Would you like to modify your selected options? (y/n) » No
Starting Lunar...
version: 1.8.9, rootDir: C:\Users\Greys\AppData\Roaming\.lunar, lunarDir: C:\Users\Greys\.lunarclient
Solar Patcher v1.7.2-PR
Built Fri Aug 19 04:27:30 EDT 2022
Attempting to read configuration from C:\Users\Greys\.lunarclient\solartweaks\config.json
Using modules ChatLimit, CloaksPlus, CustomCommands, CustomMods, FPSSpoof, HandleNotifications, LaunchRequestModule, Metadata, ModName, ModpacketRemoval, RPCUpdate, RemoveChatDelay, SolarLoaderExcluder, SupportOverlays, UncapReach, Websocket, WindowName
Launching Lunar Client

Loaded 22 finders from 7 containers!
[21:04:36] [Genesis/INFO] Launching Minecraft 1.8.9 v1_8 (parsed from 1.8.9)
[21:04:36] [IchorPipeline/INFO] Creating pipeline with [ALL, PRE_INIT, PRE_FORGE_PATCH, FORGE_PATCH, POST_FORGE_PATCH, PRE_OPTIFINE_PATCH, OPTIFINE_PATCH, POST_OPTIFINE_PATCH, INIT, INITIAL_REMAP, EXTERNAL_REMAP, PRE_META_MIXIN, META_MIXIN, POST_META_MIXIN, PRE_LUNAR_MIXIN, LUNAR_MIXIN, POST_LUNAR_MIXIN, PRE_EXTERNAL_MIXIN, EXTERNAL_MIXIN, POST_EXTERNAL_MIXIN, OBFUSCATION, FINAL]
[21:04:36] [IchorPipeline/INFO] attempting to load IchorModules using jdk.internal.loader.ClassLoaders$AppClassLoader@266474c2
[21:04:36] [IchorPipeline/INFO] found IchorModule com.moonsworth.lunar.ichor.OCIHIHHOHRHHHIIRCIOIHIRRR.CIIHRRRCHHHHICOIOCRCRRROO
[21:04:36] [IchorPipeline/INFO] found IchorModule com.moonsworth.lunar.HIOICHRRIROIOCCICRIOHCCIO.HCIIIICCOHRHCRIOIHHCRICIC.HHIIIRRHOHRHRCOHHHICRCIHC
[21:04:36] [IchorPipeline/INFO] found IchorModule com.moonsworth.lunar.CRIOHHRHICRICCIIHORIROCHC.CIIHRRRCHHHHICOIOCRCRRROO
Downloaded preview_OptiFine_1.8.9_HD_U_M6_pre1 with hash 7287fcd1a415ab87eca5e89457cc3507aa3fa579
!!! Configuration Error: expected 0bb792be16ec78d8b62586cc4856950befb3391b != downloaded 7287fcd1a415ab87eca5e89457cc3507aa3fa579
[21:04:38] [MRegistry/INFO] Running computations.
[21:04:38] [MRegistry/INFO] Running freeze/-1342028100
[21:04:38] [MRegistry/INFO] Running freeze/-917195096
[21:04:38] [MRegistry/INFO] Running freeze/1517611368
[21:04:39] [MRegistry/INFO] Finished computations in 57ms. Storing 5609438 bytes.
[21:04:39] [IchorPipeline/WARN] MappingSet for com.moonsworth.lunar.CRIOHHRHICRICCIIHORIROCHC.RCOIIHCHOIIHHOIHRIOIORCIH.HIOICHRRIROIOCCICRIOHCCIO.CCRHRHCOOIROCCIIIRIOHRIRC has 0 field mappings.
[21:04:39] [IchorPipeline/INFO] Found 1 external files and 3 IchorLoaders.
[21:04:39] [IchorPipeline/INFO] Done creating IchorPipeline in 3665ms.
[21:04:39] [Genesis/INFO] Found requested jar: C:\Users\Greys\.lunarclient\offline\multiver\natives\OptiFine_v1_8.jar
[21:04:40] [Genesis/INFO] Config hash: 83f9071b  File hash: 219a0cf2
[21:04:40] [Genesis/INFO] Found class cache: .\cache\83f9071b\219a0cf2\prebake.cache
[21:04:40] [Genesis/INFO] Loading prebaked classes...
[21:04:40] [Genesis/INFO] Loaded 5011 prebaked classes.
LUNARCLIENT_STATUS_PREINIT
[21:04:40] [Genesis/INFO] Starting game!
[21:04:41] [OptiFine/INFO] Using OptiFine namespace
[21:04:41] [OptiFine/INFO] Loaded 1050 patches.
[21:04:41] [OptiFine/INFO] Loaded 72 assets.
LUNARCLIENT_STATUS_INIT
[Bridge] Setting Bridge Implementation to com.moonsworth.lunar.RHIRICCRHOCOHCICOORRRRCIO.RCOIIHCHOIIHHOIHRIOIORCIH
[Bridge] Found textures dir: C:\Users\Greys\.lunarclient\textures
Completely ignored arguments: [--workingDirectory, ., --classpathDir, C:\Users\Greys\.lunarclient\offline\multiver\natives, --ichorExternalFiles, OptiFine-1.8.jar, --ichorClassPath, C:\Users\Greys\.lunarclient\offline\multiver\common-0.1.0-SNAPSHOT-all.jar,C:\Users\Greys\.lunarclient\offline\multiver\genesis-0.1.0-SNAPSHOT-all.jar,C:\Users\Greys\.lunarclient\offline\multiver\lunar-emote.jar,C:\Users\Greys\.lunarclient\offline\multiver\lunar-lang.jar,C:\Users\Greys\.lunarclient\offline\multiver\lunar.jar,C:\Users\Greys\.lunarclient\offline\multiver\optifine-0.1.0-SNAPSHOT-all.jar,C:\Users\Greys\.lunarclient\offline\multiver\OptiFine_v1_8.jar,C:\Users\Greys\.lunarclient\offline\multiver\v1_8-0.1.0-SNAPSHOT-all.jar]
[21:05:08] [Client thread/ERROR]: Can't find the resource index file: C:\Users\Greys\AppData\Roaming\.lunar\assets\indexes\1.8.9.json
[21:05:09] [Client thread/INFO]: Setting user: Player55
[21:05:09] [Client thread/INFO]: (Session ID is token:0:Player55)
[Bridge] Setting Minecraft Client instance to net.minecraft.client.Minecraft
[Bridge] Adding cosmetic pack to the default resource packs
[21:05:12] [Client thread/INFO]: [LC] Loaded File: Options
[21:05:12] [Client thread/WARN]: Skipping bad option: streamPreferredServer:
java.lang.ArrayIndexOutOfBoundsException: Index 1 out of bounds for length 1
        at Genesis//net.minecraft.client.settings.GameSettings.redirect$zen000$impl$loadOptions$split(GameSettings.java:3718)
        at Genesis//net.minecraft.client.settings.GameSettings.loadOptions(GameSettings.java:894)
        at Genesis//net.minecraft.client.settings.GameSettings.<init>(GameSettings.java:341)
        at Genesis//net.minecraft.client.Minecraft.startGame(SourceFile:349)
        at Genesis//net.minecraft.client.Minecraft.run(SourceFile:310)
        at Genesis//net.minecraft.client.main.Main.main(SourceFile:124)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
        at java.base/java.lang.reflect.Method.invoke(Unknown Source)
        at com.moonsworth.lunar.genesis.Genesis.main(Unknown Source)
[21:05:13] [Client thread/ERROR]: Failed to load options
java.lang.NullPointerException: Cannot invoke "com.moonsworth.lunar.HIOICHRRIROIOCCICRIOHCCIO.CIIHRRRCHHHHICOIOCRCRRROO.ORIROCRHRCRRCCOCCRCROCORH()" because the return value of "com.moonsworth.lunar.HIOICHRRIROIOCCICRIOHCCIO.IOIROOHIOHCRRHRCROCOHCCCR.OIHCOOCHIHOHHHROORROIHRIR.CHOHCHIOHHCROIROHRIHCHIOC()" is null
        at net.minecraft.client.settings.KeyBinding.wrapWithCondition$zhj000$impl$resetKeyBindingArrayAndHash(SourceFile:1015) ~[?:?]
        at net.minecraft.client.settings.KeyBinding.resetKeyBindingArrayAndHash(SourceFile:54) ~[?:?]
        at net.minecraft.client.settings.GameSettings.loadOptions(GameSettings.java:1268) [?:?]
        at net.minecraft.client.settings.GameSettings.<init>(GameSettings.java:341) [?:?]
        at net.minecraft.client.Minecraft.startGame(SourceFile:349) [?:?]
        at net.minecraft.client.Minecraft.run(SourceFile:310) [?:?]
        at net.minecraft.client.main.Main.main(SourceFile:124) [?:?]
        at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?]
        at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(Unknown Source) ~[?:?]
        at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source) ~[?:?]
        at java.lang.reflect.Method.invoke(Unknown Source) ~[?:?]
        at com.moonsworth.lunar.genesis.Genesis.main(Unknown Source) [genesis-0.1.0-SNAPSHOT-all.jar:?]
[21:05:13] [Client thread/WARN]: [OptiFine] Failed to load options
java.lang.NullPointerException: Cannot invoke "com.moonsworth.lunar.HIOICHRRIROIOCCICRIOHCCIO.CIIHRRRCHHHHICOIOCRCRRROO.ORIROCRHRCRRCCOCCRCROCORH()" because the return value of "com.moonsworth.lunar.HIOICHRRIROIOCCICRIOHCCIO.IOIROOHIOHCRRHRCROCOHCCCR.OIHCOOCHIHOHHHROORROIHRIR.CHOHCHIOHHCROIROHRIHCHIOC()" is null
        at Genesis//net.minecraft.client.settings.KeyBinding.wrapWithCondition$zhj000$impl$resetKeyBindingArrayAndHash(SourceFile:1015)
        at Genesis//net.minecraft.client.settings.KeyBinding.resetKeyBindingArrayAndHash(SourceFile:54)
        at Genesis//net.minecraft.client.settings.GameSettings.loadOfOptions(GameSettings.java:2975)
        at Genesis//net.minecraft.client.settings.GameSettings.loadOptions(GameSettings.java:1281)
        at Genesis//net.minecraft.client.settings.GameSettings.<init>(GameSettings.java:341)
        at Genesis//net.minecraft.client.Minecraft.startGame(SourceFile:349)
        at Genesis//net.minecraft.client.Minecraft.run(SourceFile:310)
        at Genesis//net.minecraft.client.main.Main.main(SourceFile:124)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
        at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
        at java.base/java.lang.reflect.Method.invoke(Unknown Source)
        at com.moonsworth.lunar.genesis.Genesis.main(Unknown Source)
[21:05:13] [Client thread/INFO]: [OptiFine] *** Reflector Forge ***
[21:05:13] [Client thread/INFO]: [OptiFine] *** Reflector Vanilla ***
[21:05:13] [Client thread/INFO]: LWJGL Version: 2.9.4
LUNARCLIENT_STATUS_INIT
[21:05:14] [Client thread/INFO]: [OptiFine]
[21:05:14] [Client thread/INFO]: [OptiFine] OptiFine_1.8.9_HD_U_M6_pre2
[21:05:14] [Client thread/INFO]: [OptiFine] Build: 20211101-204933
[21:05:15] [Client thread/INFO]: [OptiFine] OS: Windows 10 (amd64) version 10.0
[21:05:15] [Client thread/INFO]: [OptiFine] Java: 17.0.3, Azul Systems, Inc.
[21:05:15] [Client thread/INFO]: [OptiFine] VM: OpenJDK 64-Bit Server VM (mixed mode, sharing), Azul Systems, Inc.
[21:05:15] [Client thread/INFO]: [OptiFine] LWJGL: 2.9.4
[21:05:15] [Client thread/INFO]: [OptiFine] OpenGL: Radeon RX 580 Series, version 4.6.14800 Compatibility Profile Context 22.5.1 30.0.15021.11005, ATI Technologies Inc.
[21:05:15] [Client thread/INFO]: [OptiFine] OpenGL Version: 4.6.14800
[21:05:15] [Client thread/INFO]: [OptiFine] OpenGL Fancy fog: Not available (GL_NV_fog_distance)
[21:05:15] [Client thread/INFO]: [OptiFine] Maximum texture size: 16384x16384
[21:05:15] [Client thread/INFO]: [Shaders] OpenGL Version: 4.6.14800 Compatibility Profile Context 22.5.1 30.0.15021.11005
[21:05:15] [Client thread/INFO]: [Shaders] Vendor:  ATI Technologies Inc.
[21:05:15] [Client thread/INFO]: [Shaders] Renderer: Radeon RX 580 Series
[21:05:15] [Client thread/INFO]: [Shaders] Capabilities:  2.0  2.1  3.0  3.2  4.0
[21:05:15] [Client thread/INFO]: [Shaders] GL_MAX_DRAW_BUFFERS: 8
[21:05:15] [Client thread/INFO]: [Shaders] GL_MAX_COLOR_ATTACHMENTS_EXT: 8
[21:05:15] [Client thread/INFO]: [Shaders] GL_MAX_TEXTURE_IMAGE_UNITS: 32
[21:05:15] [Client thread/INFO]: [Shaders] Load shaders configuration.
[21:05:15] [Client thread/INFO]: [Shaders] Save shaders configuration.
[21:05:15] [Client thread/INFO]: [Shaders] No shaderpack loaded.
[21:05:16] [Client thread/INFO]: [LC MemoryFix] Scaling resource pack icon from 128 to 64
[21:05:16] [Client thread/INFO]: [LC MemoryFix] Scaling resource pack icon from 2048 to 64
[21:05:16] [Client thread/INFO]: [LC MemoryFix] Scaling resource pack icon from 1080 to 64
[21:05:16] [Client thread/INFO]: [LC MemoryFix] Scaling resource pack icon from 128 to 64
[21:05:16] [Client thread/INFO]: [LC MemoryFix] Scaling resource pack icon from 2048 to 64
[21:05:16] [Client thread/INFO]: [LC MemoryFix] Scaling resource pack icon from 2048 to 64
[21:05:17] [Client thread/INFO]: [LC MemoryFix] Scaling resource pack icon from 2048 to 64
[21:05:17] [Client thread/INFO]: Reloading ResourceManager: textures, Default, Alpha Bow Sound Overlay 1.8.zip, Alpha Damage Taken Sound Overlay 1.8.zip, Alpha Damage Taken Sound Overlay 1.8(1).zip, Alpha Explosion Sound Overlay 1.8.zip, Alpha Door & Chest Sound Overlay 1.8.zip, Alpha Liquid Sound Overlay 1.8.zip, Alpha Mob Sound Overlay 1.8.zip, Alpha Music Overlay 1.8.zip, -º4 Bloody Red
[21:05:17] [Client thread/INFO]: [OptiFine] *** Reloading textures ***
[21:05:17] [Client thread/INFO]: [OptiFine] Resource packs: Alpha Bow Sound Overlay 1.8.zip, Alpha Damage Taken Sound Overlay 1.8.zip, Alpha Damage Taken Sound Overlay 1.8(1).zip, Alpha Explosion Sound Overlay 1.8.zip, Alpha Door & Chest Sound Overlay 1.8.zip, Alpha Liquid Sound Overlay 1.8.zip, Alpha Mob Sound Overlay 1.8.zip, Alpha Music Overlay 1.8.zip, -º4 Bloody Red
If on Windows, make sure to provide all of the necessary dll's as specified in the twitchsdk README. Also, make sure to set the PATH environment variable to point to the directory containing the dll's.
[21:05:18] [Client thread/ERROR]: Couldn't initialize twitch stream
[21:05:18] [Sound Library Loader/INFO]: Starting up SoundSystem...
[21:05:18] [Thread-3/INFO]: Initializing LWJGL OpenAL
[21:05:18] [Thread-3/INFO]: (The LWJGL binding of OpenAL.  For more information, see http://www.lwjgl.org)
[21:05:19] [Thread-3/INFO]: OpenAL initialized.
[21:05:19] [Sound Library Loader/INFO]: Sound engine started
[21:05:20] [Client thread/INFO]: [OptiFine] Mipmap levels: 4
[21:05:20] [Client thread/INFO]: [OptiFine] Multitexture: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/0_glass_white/glass_pane_white.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/0_glass_white/glass_white.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/10_glass_purple/glass_pane_purple.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/10_glass_purple/glass_purple.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/11_glass_blue/glass_blue.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/11_glass_blue/glass_pane_blue.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/12_glass_brown/glass_brown.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/12_glass_brown/glass_pane_brown.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/13_glass_green/glass_green.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/13_glass_green/glass_pane_green.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/14_glass_red/glass_pane_red.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/14_glass_red/glass_red.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/15_glass_black/glass_black.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/15_glass_black/glass_pane_black.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/1_glass_orange/glass_orange.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/1_glass_orange/glass_pane_orange.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/2_glass_magenta/glass_magenta.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/2_glass_magenta/glass_pane_magenta.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/3_glass_light_blue/glass_light_blue.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/3_glass_light_blue/glass_pane_light_blue.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/4_glass_yellow/glass_pane_yellow.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/4_glass_yellow/glass_yellow.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/5_glass_lime/glass_lime.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/5_glass_lime/glass_pane_lime.properties
[21:05:20] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/6_glass_pink/glass_pane_pink.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/6_glass_pink/glass_pink.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/7_glass_gray/glass_gray.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/7_glass_gray/glass_pane_gray.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/8_glass_silver/glass_pane_silver.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/8_glass_silver/glass_silver.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/9_glass_cyan/glass_cyan.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/9_glass_cyan/glass_pane_cyan.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/bookshelf.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/glass.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/glasspane.properties
[21:05:21] [Client thread/INFO]: [OptiFine] ConnectedTextures: mcpatcher/ctm/default/sandstone.properties
[21:05:21] [Client thread/INFO]: [OptiFine] Multipass connected textures: false
[21:05:21] [Client thread/INFO]: [OptiFine] BetterGrass: Parsing default configuration optifine/bettergrass.properties
[21:05:22] [Client thread/INFO]: Created: 1024x512 textures-atlas
[21:05:22] [Client thread/INFO]: [OptiFine] Animated sprites: 11
[21:05:25] [Client thread/INFO]: [LC] Starting Lunar client...
[21:05:25] [Client thread/INFO]: [LC] Loading RHHHCHCOIOHROROOIROIHCCHO...
[21:05:25] [Client thread/INFO]: [LC] Loading OCIIRCROCHORIHHRHHCCHRHHC...
[21:05:26] [Client thread/INFO]: [LC] Loading RCOIIHCHOIIHHOIHRIOIORCIH...
[21:05:26] [Client thread/INFO]: [LC] Loading CORCOCHHOCIIOCRCCCOCIOHHH...
[21:05:26] [Client thread/INFO]: [LC] Loading OIHCOOCHIHOHHHROORROIHRIR...
[21:05:27] [Client thread/INFO]: [LC] Loading IHHRRCRCROOOCIROCOOHICRIO...
[21:05:29] [Client thread/INFO]: [LC] Loading OROHHHCORHHCRCCIRIRICCIHO...
[21:05:29] [Client thread/INFO]: [LC] Loading HHIIIRRHOHRHRCOHHHICRCIHC...
[21:05:29] [Client thread/INFO]: [LC] Loading HIOICHRRIROIOCCICRIOHCCIO...
[21:05:29] [Client thread/INFO]: [LC] Loading OCIHIHHOHRHHHIIRCIOIHIRRR...
[21:05:29] [Client thread/INFO]: [LC] Loading CIIHRRRCHHHHICOIOCRCRRROO...
[21:05:29] [Client thread/INFO]: [LC] Loading HRIRCRHOCCICCIOHROOCICOOC...
[21:05:29] [Client thread/INFO]: [LC] Loading HHIIIRRHOHRHRCOHHHICRCIHC...
[21:05:29] [Client thread/INFO]: [LC] Loading IICHHIOIORHIOICRCHOCOHRIR...
log4j:WARN No appenders could be found for logger (io.netty.util.internal.logging.InternalLoggerFactory).
log4j:WARN Please initialize the log4j system properly.
log4j:WARN See http://logging.apache.org/log4j/1.2/faq.html#noconfig for more info.
[21:05:30] [Client thread/INFO]: [LC] Loading CRIOHHRHICRICCIIHORIROCHC...
[21:05:30] [Client thread/INFO]: [LC] Loading IIHOCHOOHROROIHOOIROOHCIR...
[21:05:30] [Client thread/INFO]: [LC] Loading HCRCCHHRHIIIRRIRICCROCCHR...
[21:05:30] [Client thread/INFO]: [LC] Loading CRICRRHHCCOICICOCCRCIORCI...
[21:05:30] [Client thread/INFO]: [LC] Loading ORRICIOIIRROHOORORCIRHICC...
[21:05:30] [Client thread/INFO]: [LC] Loading RCRICOIOHOIOIOOOIIRICRRRI...
[21:05:30] [Client thread/INFO]: [LC] Loading OCIHIHHOHRHHHIIRCIOIHIRRR...
[21:05:30] [Client thread/INFO]: [LC] Loading CHCCHHHCORIHROHOOOROIOCIO...
[21:05:30] [Client thread/INFO]: [LC] Loading HCIHRRIRIHRRHHIRIOIHRICOI...
[21:05:31] [Client thread/INFO]: [LC] Loading OIRRROCIOOCHOCIHRRRHRHCRC...
[21:05:31] [Client thread/INFO]: [LC] Loading CIIHRRRCHHHHICOIOCRCRRROO...
[21:05:31] [Client thread/INFO]: [LC] Finished making managers.
[21:05:31] [Client thread/INFO]: [LC] Setting up listeners...
[21:05:36] [Client thread/INFO]: [LC ThirdParty] Created mod: SkyblockAddons (1.6.0)
[21:05:36] [Client thread/INFO]: [LC LANG] Couldn't get a valid language so we're setting it to ENGLISH.
[21:05:36] [Client thread/INFO]: [LC LANG] Language set as ENGLISH (en_US).
[21:05:36] [Client thread/INFO]: [LC LANG] Language file found: lang/lunar/en_US.
[21:05:36] [Client thread/INFO]: [LC Ichor] Disabling ReplayMod because there is no valid link.
[21:05:36] [Client thread/INFO]: [LC Ichor] Disabling NEU because there is no valid link.
Lunar.start
[21:05:38] [Client thread/INFO]: [LC LANG] Language set as ENGLISH (en_US).
[21:05:38] [Client thread/INFO]: [LC LANG] Language file found: lang/lunar/en_US.
[21:05:39] [Client thread/INFO]: [LC] Debugging has been disabled for ALL type(s).
[21:05:39] [Client thread/INFO]: [LC Accounts] Attempting to load account [c440027617594e57b00cb655d5bd0688]
[21:05:43] [Client thread/INFO]: [LC Accounts] Loaded content for [fx8320] Token IAT
[21:05:43] [Client thread/INFO]: [LC Accounts] Removed all accounts [0 count]
[21:05:43] [Client thread/INFO]: [LC Accounts] Starting Refreshing fx8320 with 85489369ms till expired (Valid: true).
[21:05:43] [Client thread/INFO]: [LC Accounts] Starting Refresh
[21:05:45] [Client thread/INFO]: [LC Accounts] Finishing Refreshing fx8320 (Valid: true).
[21:05:45] [Client thread/INFO]: [LC Accounts] Logging into account fx8320
[21:05:45] [Client thread/INFO]: [LC Accounts] Starting MS auth
[21:05:45] [Client thread/INFO]: [LC Accounts] After refreshing, sessions is true valid
[21:05:45] [Client thread/INFO]: [LC] Setting user: fx8320
[21:05:45] [Thread-7/INFO]: [LC Assets] Establishing connection
[21:05:45] [Thread-7/INFO]: [LC Authentication] Instantiate
[21:05:46] [Client thread/INFO]: [LC Accounts] Able to login fx8320
[21:05:47] [WebSocketConnectReadThread-70/INFO]: [LC Assets] Instantiate
[21:05:47] [WebSocketConnectReadThread-70/INFO]: [LC Auth] Connection closed (1000, "")
[21:05:48] [WebSocketConnectReadThread-78/INFO]: [LC Assets] Connection established as fx8320
[21:05:50] [WebSocketConnectReadThread-78/INFO]: [LC Assets] [] Welcome to YOUR daily dose of Solar Socket!
[21:05:51] [Client thread/INFO]: [LC] Loaded geckolib cosmetics.
Launching
[21:05:52] [Client thread/INFO]: [LC] Finished Lunar initialization.
[21:05:52] [IchorPipeline/INFO] ========= Debugging class transformation times =========
[21:05:52] [IchorPipeline/INFO] Time since IchorPipeline init: 76460ms
[21:05:52] [IchorPipeline/INFO] Time spent in IchorClassLoader.getTransformedClass(): 24232ms
[21:05:52] [IchorPipeline/INFO] classes: 43340ms
[21:05:52] [IchorPipeline/INFO] - com.moonsworth.lunar.RHIRICCRHOCOHCICOORRRRCIO.RCOIIHCHOIIHHOIHRIOIORCIH: 4394ms
[21:05:52] [IchorPipeline/INFO] - com.moonsworth.lunar.CIIHRRRCHHHHICOIOCRCRRROO.RCOIIHCHOIIHHOIHRIOIORCIH: 2086ms
[21:05:52] [IchorPipeline/INFO] - com.moonsworth.lunar.RHIRICCRHOCOHCICOORRRRCIO.OCIHIHHOHRHHHIIRCIOIHIRRR.RCOIIHCHOIIHHOIHRIOIORCIH.CIOROHOOIIIHRRHRIHRCRIORI.CIIHRRRCHHHHICOIOCRCRRROO: 805ms
[21:05:52] [IchorPipeline/INFO] - org.apache.logging.log4j.core.impl.Log4jContextFactory: 684ms
[21:05:52] [IchorPipeline/INFO] - com.moonsworth.lunar.RHIRICCRHOCOHCICOORRRRCIO.IIHOCHOOHROROIHOOIROOHCIR.CIOROHOOIIIHRRHRIHRCRIORI: 638ms
[21:05:52] [IchorPipeline/INFO] packages:
[21:05:52] [IchorPipeline/INFO] - com.moonsworth: 18507ms
[21:05:52] [IchorPipeline/INFO] - org.apache: 10105ms
[21:05:52] [IchorPipeline/INFO] - com.google: 4366ms
[21:05:52] [IchorPipeline/INFO] - com.mojang: 2295ms
[21:05:52] [IchorPipeline/INFO] - org.lwjgl: 1225ms
[21:05:52] [IchorPipeline/INFO] remapping: 32262ms
[21:05:52] [IchorPipeline/INFO] - com/moonsworth/lunar/RHIRICCRHOCOHCICOORRRRCIO/RCOIIHCHOIIHHOIHRIOIORCIH: 4334ms
[21:05:52] [IchorPipeline/INFO] - com/moonsworth/lunar/RHIRICCRHOCOHCICOORRRRCIO/OCIHIHHOHRHHHIIRCIOIHIRRR/RCOIIHCHOIIHHOIHRIOIORCIH/CIOROHOOIIIHRRHRIHRCRIORI/CIIHRRRCHHHHICOIOCRCRRROO: 668ms
[21:05:52] [IchorPipeline/INFO] - com/moonsworth/lunar/RHIRICCRHOCOHCICOORRRRCIO/IIHOCHOOHROROIHOOIROOHCIR/CIOROHOOIIIHRRHRIHRCRIORI: 637ms
[21:05:52] [IchorPipeline/INFO] - com/moonsworth/lunar/RHIRICCRHOCOHCICOORRRRCIO/OCIHIHHOHRHHHIIRCIOIHIRRR/RCOIIHCHOIIHHOIHRIOIORCIH/RCOIIHCHOIIHHOIHRIOIORCIH: 557ms
[21:05:52] [IchorPipeline/INFO] - org/apache/logging/log4j/core/impl/Log4jContextFactory: 453ms
[21:05:52] [IchorPipeline/INFO] nectar timings:
[21:05:52] [IchorPipeline/INFO] - @jdk.proxy2.$Proxy15(com.moonsworth.lunar.ichor.OCIHIHHOHRHHHIIRCIOIHIRRR.RCOIIHCHOIIHHOIHRIOIORCIH.HIOICHRRIROIOCCICRIOHCCIO,INITIAL_REMAP,CIOROHOOIIIHRRHRIHRCRIORI): 26886ms
[21:05:52] [IchorPipeline/INFO] - @jdk.proxy2.$Proxy15(com.moonsworth.lunar.CRIOHHRHICRICCIIHORIROCHC.RCOIIHCHOIIHHOIHRIOIORCIH.HIOICHRRIROIOCCICRIOHCCIO,POST_OPTIFINE_PATCH,CCRHRHCOOIROCCIIIRIOHRIRC): 6724ms
[21:05:52] [IchorPipeline/INFO] nectar matches:
[21:05:52] [IchorPipeline/INFO] - @jdk.proxy2.$Proxy14(com.moonsworth.lunar.CRIOHHRHICRICCIIHORIROCHC.RCOIIHCHOIIHHOIHRIOIORCIH.CIIHRRRCHHHHICOIOCRCRRROO,OPTIFINE_PATCH,CIIHRRRCHHHHICOIOCRCRRROO): 6397
[21:05:52] [IchorPipeline/INFO] - @jdk.proxy2.$Proxy14(com.moonsworth.lunar.CRIOHHRHICRICCIIHORIROCHC.RCOIIHCHOIIHHOIHRIOIORCIH.HIOICHRRIROIOCCICRIOHCCIO,POST_OPTIFINE_PATCH,HCRCCHHRHIIIRRIRICCROCCHR): 6396
[21:05:52] [IchorPipeline/INFO] - @jdk.proxy2.$Proxy15(com.moonsworth.lunar.CRIOHHRHICRICCIIHORIROCHC.RCOIIHCHOIIHHOIHRIOIORCIH.HIOICHRRIROIOCCICRIOHCCIO,POST_OPTIFINE_PATCH,CCRHRHCOOIROCCIIIRIOHRIRC): 6396
[21:05:52] [IchorPipeline/INFO] - @jdk.proxy2.$Proxy15(com.moonsworth.lunar.ichor.OCIHIHHOHRHHHIIRCIOIHIRRR.RCOIIHCHOIIHHOIHRIOIORCIH.HIOICHRRIROIOCCICRIOHCCIO,INITIAL_REMAP,CIOROHOOIIIHRRHRIHRCRIORI): 2406
[21:05:52] [IchorPipeline/INFO] - @jdk.proxy2.$Proxy14(com.moonsworth.lunar.HIOICHRRIROIOCCICRIOHCCIO.HCIIIICCOHRHCRIOIHHCRICIC.RCOIIHCHOIIHHOIHRIOIORCIH,PRE_LUNAR_MIXIN,RCOIIHCHOIIHHOIHRIOIORCIH): 2398
[21:05:52] [IchorPipeline/INFO] ========================================================
// class version 53.0 (53)
// access flags 0x1
public class com/grappenmaker/solarpatcher/generated/Utility implements com/grappenmaker/solarpatcher/util/generation/IUtility {


  // access flags 0x1
  public displayPopup(Ljava/lang/String;Ljava/lang/String;)V
    INVOKESTATIC com/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO.HCIHORRHOOHOHHIIROOOOCHOI ()Lcom/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO;
    GETFIELD com/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO.RCOCHRRIHHCCHCORCIOIHOIRI : Lcom/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO/RCOIIHCHOIIHHOIHRIOIORCIH;
    NEW com/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO/RCOIIHCHOIIHHOIHRIOIORCIH/RCOIIHCHOIIHHOIHRIOIORCIH/CIIIROCOIIOHOCHOOCICRCIOI
    DUP
    ALOAD 1
    ALOAD 2
    INVOKESPECIAL com/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO/RCOIIHCHOIIHHOIHRIOIORCIH/RCOIIHCHOIIHHOIHRIOIORCIH/CIIIROCOIIOHOCHOOCICRCIOI.<init> (Ljava/lang/String;Ljava/lang/String;)V
    INVOKEVIRTUAL com/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO/RCOIIHCHOIIHHOIHRIOIORCIH.RCOIIHCHOIIHHOIHRIOIORCIH (Lcom/moonsworth/lunar/HIOICHRRIROIOCCICRIOHCCIO/CIIHRRRCHHHHICOIOCRCRRROO/RCOIIHCHOIIHHOIHRIOIORCIH/RCOIIHCHOIIHHOIHRIOIORCIH/CIIIROCOIIOHOCHOOCICRCIOI;)V
    RETURN
    MAXSTACK = -1
    MAXLOCALS = -1

  // access flags 0x1
  public getClientBridge()Ljava/lang/Object;
    GETSTATIC com/moonsworth/lunar/CIIHRRRCHHHHICOIOCRCRRROO/CIIHRRRCHHHHICOIOCRCRRROO.CIOROHOOIIIHRRHRIHRCRIORI : Lcom/moonsworth/lunar/CIIHRRRCHHHHICOIOCRCRRROO/HHIIIRRHOHRHRCOHHHICRCIHC/HIOICHRRIROIOCCICRIOHCCIO;
    ARETURN
    MAXSTACK = -1
    MAXLOCALS = -1

  // access flags 0x1
  public getVersion()Ljava/lang/String;
    INVOKESTATIC com/moonsworth/lunar/CIIHRRRCHHHHICOIOCRCRRROO/CIIHRRRCHHHHICOIOCRCRRROO.getMinecraftVersion ()Lcom/moonsworth/lunar/OHOHCHRCIOIHIOCROHIIIIIRO/RCOIIHCHOIIHHOIHRIOIORCIH;
    INVOKEVIRTUAL com/moonsworth/lunar/OHOHCHRCIOIHIOCROHIIIIIRO/RCOIIHCHOIIHHOIHRIOIORCIH.toString ()Ljava/lang/String;
    ARETURN
    MAXSTACK = -1
    MAXLOCALS = -1

  // access flags 0x1
  public <init>()V
    ALOAD 0
    INVOKESPECIAL java/lang/Object.<init> ()V
    RETURN
    MAXSTACK = 1
    MAXLOCALS = 0
}
Sent launch request
LUNARCLIENT_STATUS_STARTED
[Bridge] Using OptiFine wrapper
[21:05:53] [Client thread/INFO]: [OptiFine] *** Reloading custom textures ***
[21:05:53] [Client thread/INFO]: [OptiFine] Enable face culling: acacia_leaves, birch_leaves, dark_oak_leaves, jungle_leaves, oak_leaves, spruce_leaves
[21:05:59] [Client thread/WARN]: Unable to play unknown soundEvent: minecraft:music.menu
```
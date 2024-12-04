Some of descriptions are from `READ_ME.txt` written by JB himself.

# Using arguments
Simplest way to pass arguments (AKA launch arguments) when launching any executable is to create it's shortcut, select it, right-click, then press "Properties", and edit "Target". Arguments are string values separated by spaces, and there should be space after path to .exe, like this:

![<Here should be image of shortcut's properties, but it's not displayed for some reason>](Images/ShortcutProperties.png)

Braid reads arguments without order, the only thing which matters is that values for arguments with values should be right after those arguments.

# Toggles
Those arguments usually just toggle something, to use them just place them anywhere.
For example: `-editor`.

`-editor` - Allows you to use all hotkeys. Hotkeys list: [Hotkeys](Hotkeys.md)

`-no_package` - Uses data from folders instead of zips. Use this when you're making a mod, so that your changes are saved.

`-windowed` - Starts the game in windowed mode. Keep in mind that you can't move window while braid is focused, because you can't get mouse of bounds, so you either need to start it and then instantly move mouse to top of screen, and get right moment to start dragging window, or you need to have some other windowed app (f.e. calculator) focused above braid, and while it's focused you can drag braid's window. If you don't specify this option, you can switch between fullscreen and windowed at runtime by pressing Alt-Enter.

`-60fps`, `-30fps`, `-20fps`, `-15fps`, `-12fps`, `-10fps` - Bypass Braid's startup frame-rate check and force the game to try and run at this many frames per second.  If the number is too high for your computer, action in the game will be slowed down.  Because you are skipping the startup test, postprocessing will always be on.  If you want to turn it off (and thus possibly hit the frame rate target you are going for), use -no_post below.  If you press the 0 key in-game, you'll get some HUD text telling you what frame rate the game is trying to hit, how fast it is actually going, and whether postprocessing is turned on.  

`-no_post` - Do not perform postprocessing effects.  This may make the game run more quickly on your graphics hardware, but time-oriented visual effects will be much simpler. (Instead of chrome change (grey/colorful screen) screen will be overlayed with blue/yellow colors)

`-no_music` - Disable music.  

`-no_vsync` - The game will not synch to the vertical refresh.  This may allow the game to run a little faster, but you will see tearing in the image.


# With values
Those arguments require some value passed. Add value as next argument.
For example: `-width 1920`.

`-language <string>` - Changes game's language to specified one. If you do not use one of these options, Braid will read the appropriate language setting from Windows (or from Steam if you are using Steam). Values allowed by default: `english`, `french`, `german`, `italian`, `japanese`, `korean`, `polish`, `portuguese`, `russian`, `spanish`, `tchinese`, `czech`\*, `georgian`\*.  
\*Unofficial translations. Info is based on files in `data/strings/`, and may be inaccurate.

`-width <number>`/`-height <number>` - Starts game with specified window width/height.

`-universe <string>` - Loads universe from `Braid/universes/` folder, or crashes if specified folder is not found or is corrupted.
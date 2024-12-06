This file will list all known hotkeys for braid. Keep in mind that most of those keybinds are found by clicking random buttons, so list probably doesn't have all avaible keybinds.

# Don't require editor
`F1` - Move to levels selector from level, or to house from levels selector. Will show confirmation screen, unless it's disabled. (see below)

`F2` - Used in screen which appears after pressing `F1`, to disable world exit confirmation forever.

`0` - Toggles debug info about fps, postprocessing and window info.

`PrintScreen` - Take a screenshot and save it in the Braid folder.  You must have write permission to the Braid folder for this to work. (Based on READ_ME.txt from JB, didn't manage to get it working)

# Require editor
Hotkeys listed here require `-editor` argument. See [Enabling Editor](EnablingEditor.md) for more info.

`F9` - Toggle particle's generation seed (Probably?).

`F10` - Pause game.

`F11` - Open editor. If editor wasn't open in this game launch will open current world in editor.

`Shift+F11` - Open some window with animations. 

`[` and `]` - Go to previous/next level in this world. F.e. when you use it in `world0-0` you go to `world0-1`. Very useful.

`L` - Restart level. This also loads latest version, so when you're using [`-no_package`](LaunchArguments.md) you can load version you just saved. Equal to `[` then `]`.

`Ctrl+I` - Load `save` world. That world is created each time you press `F11`, and contains current world state. Equal to `load as..` > `save`.

`P` - Pauses game. Has higher priority than `F10`, and persists after opening pause menu (`esc`).

`T` - Puts a pink box on the screen. Purpose unknown.


## Editor controls

`WASD` - Move camera.

`Left-click` - Select entity. Adds to selection when used with `Shift`

`Ctrl`+`C`/`V` - copypaste entity. You can copypaste entities from world to world, but not from one game's window to another.

`F8`/`G` - Deselect entity.

`Q` - Changes border of selected entity from orange to blue. Purpose is not exactly knows, but I've noticed that when you try to resize "pieced image" you move it. When you using blue selection you cut it instead.

`E`/`R` - Decrease/Increase depth value of selected entity by 1. Changes depth by 10 if `Shift` is hold.

`Ctrl+G`/`Shift+G` - Selects all entities similar to selected one. I don't exactly know which entities are "similar".

`PageUp` - (???) Zooms out background layer a bit, like when you rewind. On second press slowly zooms it back.

`J`/`L` - Previous/Next entity (by ID).

`Ctrl+WASD` - Moves selected entity a bit.

`Shift+WASD` - Moves selected entity a bit more.

`H` - Hide **hovered** entity.

`Shift+H` - Unhind all entities.

`Shift+C` - Change visible layer to `Collision`.  
`Shift+P` - Change visible layer to `Particles`.  
`Shift+F` - Change visible layer to `Foreground`.  
`Shift+B` - ~~..obvious, isn't it?~~ Change visible layer to `Background`.

Hold `Alt` to see all entities, no matter which layer is currently visible. Doesn't show hidden entities.
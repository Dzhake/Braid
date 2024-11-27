# Extracting braid's data
Go to `Braid/data/`, find there file `package.braid`, rename it to `package.zip`, and unzip it with any zipping software.

You should have a bunch of folder in `Braid/data/` now.

# Creating your universe

Now, create `universes` folder next to `data`. Create there folder with name for your future mod. You can always change it later.

Copypaste `All.variables`, `level_config` and `entities/` from `Braid/data/` to `Braid/universes/<your universe>`.

Now you should be able to launch the game with `-no_package -universe <your universe>`, and if you edit something and then press `Save` the changes should be saved.

Braid will only read `world..` files from your mod, so you can't replace vanilla entities or menus. Tho you can edit them, and then copypaste in your `Braid/data/entities` folder. But keep in mind other people won't have it replaced.

# Packaging universe

Once you want to share your universe with others, you need to package it. To do that, create folders `universes/<your universe>` anywhere, then copypaste your `Braid/universes/<your universe>/data` there. Zip that, and rename it to `package.zip`. To use it people need to put `package.zip` in `Braid/universes/<your universe>`, and use `-universe <your universe>`.

I know I'm pretty bad at explaining it (?). In the end you should have this file structure: `Braid/universes/<your universe>/package.zip`, and `package.zip` should have these folders: `universes/<your universe>/data/`.

# Related guides

For more info about editing universes see other guides here. Probably you should start with `Hotkeys`.
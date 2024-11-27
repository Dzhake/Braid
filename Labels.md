Every entity has labels. I don't know if entity can have more than one label. I think you can invert any label which checks for something by adding `!` before it. F.e. `!solved 2`.

List of all known labels:

# universal

`:lightswitch` - Used with `Marker` entity. Pass unique (per-level) ID as `argument` value. Entities with `#<your value>` will appear only when you walked past middle (to the right) of your `Marker`. (F.e. see `bathroom` in `world0-0`).

`:guy_backlit` - Requires two entities (markers? TODO: check). Tim will look like shadow between them (used in `world0-0`).

`solved <X>` - Entity will only appear if puzzle for that world is completed. Used in `world0-0` for ladder.

`unsolved <X>` - Like `solved`, but entity will appear only if puzzle is not completed.

`#<Literally anything ever>` - Entity will show (and probably will be collidable? TODO: check) only when value after `#` is active. F.e. see `:lightswitch` above.

`letter` - To create letters like in the start of `world0-0` you need to create `Surface` with some label (gonna call it `X`). Then, create `Particles` with label `letter`, and `path_source` (page 5, 3rd from top) - `X`.

`:dissolve_title` - Probably stops particles with label `letter` from spawning? (TODO: check)

Give `Switch` and `Platform` same label to connect them.

# Level-specific (?)

## World0-0

`1-6` as labels for `Markers`. Those spawn doors which go to `world0-<label>`.

`#<2-6>` used to "turn lights on" for specific worlds. (You know how background flashes when you unlock new world)



## Level selectors (world0-..)

`:paragraphs`. Purpose unknown.

`doors` will spawn doors which lead to levels of that world. Probably based on `level_config`? (TODO?)
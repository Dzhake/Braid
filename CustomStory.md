Unfortunately the game doesn't read custom `strings/` files, so you can't just replace all the text you want.
Instead, you have to write the text directly.

Any book requires `Text` entity with `driven_by_story_page` checked.
I Also recommend to check `no_pixel_snap`, because for some reason text looks WAY better if you check it.

Then, you need `Story Page` entity. Instead of `story_name`, which uses text ID in vanilla, you write all the text directly.

Yes, strings editor in braid's editor is awful.
Double check your text before writing, because if you need to fix *any* small typo you need to rewrite everything after that typo.
And you need to delete every single symbol after that typo, one by one, you can't just hold backspace.

You can also create `Story Page`s with empty `story_name` to hide text.
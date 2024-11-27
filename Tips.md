This is just a random collections of tips.

`make exempt` flag only spawns particles on top part of entity (about 1/4 of it). You can use invisible not collidable block if you want to spawn those particles in specific area.

Changing entity flags or hiding entities are not saved as separate undo step, and are undone when you undo next action. You can change `entity_flags` field manually instead, to save it.

When you stop hovering text field you stop inputting text there.

Paradigm is the entity used to change time behaviour.

You can copy entities from one world to another. I prefer copying instead of creating entities.

Labels are very important. More about them here: [Labels](Labels.md)
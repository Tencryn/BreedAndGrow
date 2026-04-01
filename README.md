# BreedAndGrow
Hytale currently does not allow NPCs to grow and breed, and I decided to **challenge** myself to learn NPC behaviours and add them myself.

## Dependencies
- https://github.com/Tencryn/NPCExtras

## Warning
This mod modifies all Livestock NPCs alongside `Template_Animal_Neutral.json` and `Template_Livestock.json`, and will likely conflict with other mods that modify the same files.

**The intention is for this implementation to be as vanilla-like as possible.**

## Ageing
Vanilla NPCs do age in accordance to world time, but babies do not grow into their adult form.
- Livestock young will grow into adults between 7 and 14 days
- Growth cannot be disabled at this time

## Breeding
Breeding takes advantage of the current food system, and works similar to how it does in Minecraft.\
It is a primitive system that is not perfect, and relies heavily on flags to avoid unnecessary offspring.
- Only tamed Livestock can breed
- If an NPC cannot find a suitable mate, they will become the "Birth Giver"
- Birth Givers do not search for a mate, and cannot breed with other Birth Givers
  - If you have two NPCs that aren't breeding, it is likely due to this and you will have to wait until you can feed them again

# Stardew Modded Skill Prestige Patch for Sword & Sorcery

This is a fix for players using the [Skill Prestige Unofficial Fix for 1.6.15](https://www.nexusmods.com/stardewvalley/mods/30635), the SpaceCore Adapters from that mod's additional files, and the mod [Sword & Sorcery](https://www.nexusmods.com/stardewvalley/mods/12369).

Currently there is a bug which hardlocks your save if gain level 4 in the Sorcery/Witchcraft skill on any pass through the skill after the first. This is because the Crafting recipe for "Teleport Circle" is never removed. When the game tries to add it again, it fails. You cannot leave the level up screen, cannot save, and cannot progress.

## What this patch does

At the end of each day, it checks if your Witchcraft skill is less than 4 and if you know the Teleport Circle recipe. 

If both criteria are true, it removes the Teleport Circle from your known recipes.

You should not know the recipe at that point in a prestige so removing it at these low levels does nothing harmful. Sword & Sorcery will regrant it every time you hit level 4.

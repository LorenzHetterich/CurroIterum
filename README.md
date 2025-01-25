# CurroIterum
Minecraft mod that turns the game into a rouge-like experience.

While deciding on a name for the mod idea, I found the following very cool data pack with a similar idea (that I am **NOT** affiliated with in any way):
https://modrinth.com/datapack/rogue-craft
It's a lot of fun, so feel free to check it out :)

The basic idea is to implement an adventure system similar to those in isekai animes (adventurers that have an adventurer rank they can increase; they can accept missions based on their rank; when they complete missions they get rewards and can increase their adventurer rank).
The missions will create a new dimension where players have to finish a set of tasks (like kill certain monsters, collect certain resources) to finish it.
Then, players get rewarded with money that they can spend on permanent updates (e.g., recipes for mods which are all disabled by default) or updates that apply to missions (e.g., starting items, starting mod recipes).
Players also get rewarded with adventure xp to increase their adventurer rank.

## Detailed Idea
The Idea is to remove recipes (crafting recipes, but also furnaces and modded machines like Mekanism Crushers, etc.) using dynamically created datapacks.
Then, everyone in the server can start a **mission** together.
For this, the players may choose a mission from the quest board that they can complete with their current adventurer rank.
A mission will consist of world and environmental parameters (e.g., void world generation, nether-like world generation, always daytime, etc.), one ore multiple tasks (e.g., collect 1k Iron Ingots, defeat the ender dragon, etc.), and some modifiers (e.g., start with two random additional mods fully unlocked, start with only 4 hearts, ...).
Depending on the difficulty, each mission has a random minimal required adventure rank (F, E, D, C, B, A, S, maybe more coming later), a fix amounnt of rewarded adventurer xp, and a variable amount of monetary reward depending on which tasks are completed (some of them might be optional).
When a mission is selected, a new dimension according to the mission parameters is generated using a data pack and all players are teleported into this new dimension (with an empty inventory / whatever starter items they are supposed to get).
In this dimension, they must now complete the mission by completing at least all required tasks to leave, or they can give up and loose some adventurer xp.
(Some missions might also be hardcore. If all players die, the mission is automatically given up.)
once all required tasks are completed, the mission can be completed.
Then, the players are teleported back into the overworld, and the dimension that was created for the run is deleted.
The players are awarded with the adventurer xp as well as the monetary reward.
Now they can spend some of the coins for permanent unlocks for runs (e.g., start with all recipes for a random mod unlocked on each run, start with a diamond pickaxe, start with a wind generator, start with one additional heart, start with some recipes of a specific mod unlocked, ...).
Unlocking recipes for a fixed mod will also unlock these recipes for the overworld.
Additionally, some unlocks can be made for the normal minecraft overworld.
Thus, completing run also progresses the overworld.

If I get some system that allows unlocks per-player to work (which I'm not sure I will be able to), the progress might not be shared amongst all players on the server, but players can create teams which enter missions together and share some of the progress.
The adventurer xp would still be per-player (e.g., each player has its own adventurer rank) and the group can only acceppt missions that the highest adventure rank player in the group could accept.
However, I don't think there will be any restrictions on group construction (like a maximum difference in adventure rank), but lower adventure level players will receive less adventure XP for missions that are way above their level.

## Development Progress
Not Started

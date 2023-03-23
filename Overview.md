---
tag: Game
---

1. Introduction: This document is a concept of a game that is meant to theorize what a game designed from the ground up for the (current) higher-end of VR hardware would look like. I'm basing the formatting off of the GTA GDD ([[../Resources/grand-theft-auto.pdf]])
	1. Scope: This is document is written partly for fun, and partly for an actual plan that I (Toast) have in mind for a game I would like to make in the future.
	2. Type Conventions: Parenthesis, or (), will be used the same as normal (asides from the normal sentence, in my writing I use these a lot, and I often end up turnig the parenthesized content into other pages, so feel free to comment on run-on parenthesis), for personal habit reasons. Square Brackets, or [] will be used as a way of indicating unfinished, or undetermined information / content. Curly Brackets, or {} will be used as [I hope I don't need to use these, as then we're getting into a really annoying territory]

2. References
	1. Sword Art Online Season 2
	   [I didn't have internet when I was writing this, *please don't forget to put the actual citation in*]

3. Specification
	1.  Concept
	   The aim of [[Game Name Here]] is to create an open-world, Virtual Reality (VR) Shooter that is an immersive, polished, and "detailed" experience (Detailed being in quotes, due to the art style being currently up in the air), using the higher end of VR hardware to create an amazing physical experience.
	2. Story
		- The story is set in a post-apocalyptic Cyberpunk-ish world.
	3. Game structure
	   The world of [[Game Name Here]] will have an expansive explorable map, with new environments being added, and modified as players go through the experience. Along with the regular overworld, there are a bunch of separate instances (For more information on competitive instancing, consult [[Server Infrastructure]]) designed for Ranked Play. 
	4.  Players
	   The game will be playable by [currently undetermined amount of players (This number depends on hardware performance and speeds, and I don't have an estimate currently)] players simultaneously, in 2 [or three] servers across the United States [Shh, I have plans for servers abroad]. (For more information, see [[Server Infrastructure]])
	5. Action
	   Players will be able to run, walk, and shoot (and maybe drive?), across various types of terrain, and environments, no form of navigation assistance is given [this decision is not final]. Players are encouraged to explore not through scripted missions, and more of a springboard to encourage players to seek out missions set out by other players, or to set their own goals. 
	6. Objective
	   The objective is to be the very best (that no one ever waaaas), on BP Leaderboards (Bullet Points [name not final] for more information on BP, see [[Bullet Points]]), and on Competitive Leaderboards.

4. Graphics 
	1. Landscape
	   The landscape will be viewed in first person inside a VR headset. The world (as previously mentioned), will be set in a futuristic cyberpunk-esque world, with a lot of dystopian tones the further you go from the main cities, with many smaller cities and towns being abandoned, and desolate (There are a few of these desolate cities that will be sized considerably larger than the ones that currently dominate the skyline for gunfight variability). 
	2. Detail, and performance issues
	   To keep the game looking visually stunning, and as "realistic" as possible, I would like to make the render distance quite large. In order to achieve this, a few visual downgrades will be made to keep the game looking good while not sacrificing the grand size that this world will have [Look into some optimizations that Breath of the Wild made to keep it playable].
	3. Art Style
	   While a definitive answer for the art style this game will have has not been decided, a Cel-Shaded art style would have many visual advantages in terms of performance, and would be a distinctive look for a VR shooter, as often they go for a 'gritty realism' present in other FPS'.
	4. Display (User Interface)
	   The plan is to keep the visuals as minimal as possible while giving all necessary information to the player and, as mentioned before, customization is to be considered (meaning the UI does not have to be the end all-be-all for every player). It is planned to have two UI elements turned on by default:
	   - Health: This is a single bar presenting the players health shown in the top left corner of the player's vision.
	   - Ammo: This is a number presenting the number of bullets left in the currently held weapon , along with a smaller number showing how many magazines or 'reloads' a player has for the held weapon, shown on the bottom right hand of the player's vision; additonall, there is also a bar below the bullet count showing the amount of ammo left in the current reload.
	   Additionally, popups for when a player recieves a message in the bottom left-hand corner of their vision. (All of this is configurable, and subject to change)
	5. Weather / Time
	   Players can experience weather anywhere from clear weather to monsoon, and anything in-between. This has a visual, and strategic impact on how players traverse, and fight.
	   The game also has a Day-Night cycle based off of real world time, and requires players to change their loadouts accordingly.
	   
5. Data Storage
	1. Destruction and, Environmental Changes
	   The overworld will most likely not be hardcoded onto a player's hardware (players might have the option to turn off location 'caching', or manually download areas), 
	   [This is a theoretical mechanic that may be too demanding, or require too many requests to be viable for a stable experience]
	   Players can alter the overworld environment in ways that change the playing field in semi-permanent ways (This data does not need to be stored for Instances, due to them being cleared once the match is over). Some examples of this are:
	   - Blowing up or otherwise destroying enough support for a building to collapse, causing the building, and surrounding structures to be modified [Can you see where the potentially insane amount of demand comes from?], and changing the combat environment.
	   - Corpses? Decay?
	   - Blood stains, bullet holes, bullet shells, discarded magazines, etc. appear as remains of gunfights, and as loot. 
	 2. Metadata
	    1. Player statistics such as BP, Kills, etc. are accessible to them and other players through the game client, website, as well as in game.
	    2. Along with statistics being stored for each player, the player's weapons have metadata for Kills, reloads, and previous owners. Weapons are customizable, and nameable.
	    3. Death messages / Graves?

6. Target System
   This game will be targeting mid, to high-end gaming computers, with high-speed storage, and higher-speed network connectivity being the major requirement to keeping this game running smoothly, and beautifully. 

7. Development System
   While a solid answer has not been yet given, the engine of for this project is one of three options:
   -  Unity: An all around engine, designed for all sorts of projects, and visual styles
   - Unreal engine: A primarily 3D engine designed for realism, and cutting edge-visual features
   - Godot: [I don't know too much about this engine and I may remove this one from the list]
8. Gameplay (Oh goodie, the section everybody has been waiting for)
	1. World
		1. The Overworld
		   The game world will be huge, with a specific focus on filing it with personality, and detail, each environment will be hand-crafted to suit the theming, and mood of each area. [Whether or not to provide the player with a map in-game is up in the air]
		2. Instances and Maps
		   These areas designed for small casual skirmishes, and ranked play will come in varying sizes, from a small warehouse to a large park. Maps do not need to be visually consistent with the rest of the game, (For canon reasons, instances are considered simulations, players are essentially in the hunger games). As such, some examples of themes could be:
		   - In a tube station
		   - A hospital
		   - A (canonically) fictional city 
		   - On top of (or inside of) a train
		   - In a plane
		   - Depot
	1. Landscape
	   The landscape will consist of:
	   - Cities
	   - Armories
	   - Airfields
	   - Bus terminals (Because why not?)
	   - And destroyed versions of all of the above
	   - And each also is contained within a biome of some sort
	3. Environments / Biomes
	   These include:
	   - Wasteland (Either by nuclear, or some other disaster)
	   - Pasture
	   - Desert
	   - Tundra
	   - Forest
	     There does not have to be only one environment type per area.
9. Frontend
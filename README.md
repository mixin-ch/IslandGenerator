# Minecraft Island Generator Plugin

## Create your custom islands in every world!
Recommended to use in void worlds, but can also be used in others.

On every island a chest will be spawned, which when clicked, will drop loot.
The content multiplier can be modified via the config.yml.

Should the server overload, try setting the "tickBuffer" in the config file to a higher number, to give the server the oppertunity to relax.

## Plugin Guide (English)
[![](https://img.youtube.com/vi/vfwuMaA8BqY/0.jpg)](https://www.youtube.com/watch?v=vfwuMaA8BqY)

## Commands
`/mx-ig reload`
Reloads the plugin.

`/mx-ig generate`
Generates the islands within <x>*<x>*<x> cube defined by "spawnRadius" in the config file.
This will not override existing Islands.
You can increase "spawnRadius" and generate again, to expand the world.
This can take a while.

`/mx-ig regenerate`
Removes all existing islands, which are unlooted, and generates them again.
This will remove blocks built on them.
It will do nothing, if the island chest is looted.
This can take a while.

`/mx-ig lookupLoot`
Shows the percentage of chests looted in the world.

`/mx-ig config <key> <value>`
Sets the value of the config file.
possible keys:
- tickBuffer (integer >= 0)
- lootMultiplier (number >= 0)
- spawnRadius (integer >= 1)
- islandDistance (integer >= 1)
- islandRadius (integer >= 1)
- maximumHeight: (integer)
- minimumHeight: (integer)
- worlds (can have multiple values)

## Permissions
islandGenerator.*
Includes all other IslandGenerator permissions.
default: op

islandGenerator.reload
/mx-ig reload
default: op

islandGenerator.generate
/mx-ig generate
/mx-ig regenerate
default: op

islandGenerator.lookup
/mx-ig lookupLoot
default: op

islandGenerator.config
/mx-ig config
default: op

## Config
Default:
spawnRadius: 100
islandDistance: 50
islandRadius: 20
tickBuffer: 1
worlds:
- world
maximumHeight: 255
minimumHeight: 0
lootMultiplier: 20

spawnRadius <x>
All islands generated will be within a <x>*<x>*<x> cube.

islandDistance <x>
The centers of the islands have a minimum of <x> blocks distance to each other.

islandRadius <x>
The average radius of an island is <x> blocks wide.

tickBuffer <x>
The generator waits <x> ticks after every generated island, so the server wont be overloaded.

worlds
All the worlds affected by the IslandGenerator.

maximumHeight <x>
Islands will spawn on at most Y = <x>.

minimumHeight <x>
Islands will spawn on at least Y = <x>.

lootMultiplier <x>
How much loot will be generated by the chests.
The average value will be <x> iron bars.
  
## Support
If you have any questions, you can
- join our Discord
- write down in the comments of the Video Review

## Recomended plugins
Mixed Catastrophes:
https://www.spigotmc.org/resources/mixed-catastrophes.92702
Use this plugin for more depth and a challanging expirience.
Interactions with this plugin comming soon.

Holographic Displays:
Each island has a randomly generated name, this plugin will display it.
https://dev.bukkit.org/projects/holographic-displays


More of our Stuff
Join our minecraft server: Mixin.ch
Where you can experience our plugins in action.

Join us on Discord:
https://discord.com/invite/rpUcsgfpX6

Check out our YouTube-Channel for News, Future Updates and Entertainment! :D
https://www.youtube.com/channel/UCCcXjZeFvFORbK7zhy0maZw

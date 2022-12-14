# ProdigyBot 
A bot for CMPUT 350 at UAlberta. ProdigyBot follows the same running process as [BasicSC2Bot](https://github.com/solinas/BasicSc2Bot).
ProdigyBot uses a simple 4-gate rush to attack the enemy around the 3:30s mark. If the rush is successful, the army will begin attempting to "sweep" the enemy 
base for any stray buildings. The build order used is a direct implementation of HuShang's 4-gate tutorial, [see his video here for more details](https://www.youtube.com/watch?v=F_C9Vqv6lFE).

Created by Gerard Van Genderen, Bennett Wiredu, Dave Goel, and Aidan Lynch.
Thanks to Devon "HuShang" Prefontaine and Josh Lucas for their help and advice while creating the bot.

# Install Instructions
## Requirements
* Starcraft 2 ([Windows](https://starcraft2.com/en-us/)) 
* [Starcraft 2 Map Packs](https://github.com/Blizzard/s2client-proto#map-packs)

The following maps are supported: BelShirVestigeLE, ProximaStationLE, and CactusValleyLE. Place the .SC2Map files in `.../Program Files (x86)/StarCraftII/Maps`, and create the Maps folder if it
does not exist.

For convenience, two executables have been provided:

* one for playing against ProdigyBot yourself.
* one for playing against ProdigyBot on the Sc2LadderServer, if you'd like to run your own bot against ours. You can also run this executable against the built-in AI (see below).

Note that the executables were compiled on Windows, so they will not work on Mac or Linux.

For playing against ProdigyBot yourself, make sure you've installed the required maps. Then you should be able to simply run the executable, and two instances of Starcraft should open.

# Playing against the built-in AI

In addition to competing against other bots using the [Sc2LadderServer](https://github.com/solinas/Sc2LadderServer), this bot can play against the built-in
AI by specifying command line argurments.

For example,

```
/SC2ProdigyBot.exe -c -a zerg -d Hard -m CactusValleyLE.SC2Map
```

will result in the bot playing against the zerg built-in AI on hard difficulty on the map CactusValleyLE.

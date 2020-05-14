[comment credits-readme-install-instructions]

Created by Soulless
compiled from Neruns distro from RUNUO
Thanks to AmonVangrell for inspiring me to make this

VERSION 1.0.1
-fixed some errors causing issues with correctly adding spawns

VERSION 1.0.2
-fixed issues with spawns not wanting to spawn their full array of creatures.
-fixed issues with home and homedist
-
VERSION 1.0.3
-fixed duplicate doors on felucca/trammel britain bank
-benefactor of britain is now a t_normal type
-added uoclassic spawns for those who want an older pre T2A server	(.spawn_uoclassic command)
-fixed sysmessages for signs/doors/moongates generation/removal

VERSION 2.0.a
-Redid the spawner dialog, a lot less messy in the scripts, decoration menu next.
-I've reverted back to the 56b base scripts for my server, as I require nothing more than that. I will include both 56b & 56c defs in future releases.
-added check to skip different stages of Magincia based on reported client version
  *Old Magincia [Client <= 6.0.3.1]
  *Magincia Ruins [Client >= 6.0.4.0 && Client <= 7.0.13.0]
  *New Magincia [Client >= 7.0.13.1]
//do not spawn signs, doors, deco, npcs in cities that have been altered by the client
-Redid the decoration dialog gump, added individual decoratin buttons for each facet and its areas
-added a counter on the individual buttons to show what places have been spawned/decorated x many times
doors will now all be double linked after being generated
-shop signs will now bear the name of the room_def they are adjacent to


***************************************************
****************INSTALL INSRUCTIONS****************
***************************************************

go into the woldgen/spawns/ folder and select the correct spawner_defs.scp and uncomment the ".56*" extension. 
You will need to select one of these  or make a custom spawner def that matches up with your chardefs


place this in your spheretables :
scripts/custom/worldgen/
scripts/custom/worldgen/spawns/
scripts/custom/worldgen/spawns/felucca/
scripts/custom/worldgen/spawns/trammel/
scripts/custom/worldgen/spawns/ilshenar/
scripts/custom/worldgen/spawns/malas/
scripts/custom/worldgen/spawns/tokuno/
scripts/custom/worldgen/spawns/termur/
scripts/custom/worldgen/decoration/
scripts/custom/worldgen/decoration/felucca/
scripts/custom/worldgen/decoration/ilshenar/
scripts/custom/worldgen/decoration/malas/
scripts/custom/worldgen/decoration/misc/
scripts/custom/worldgen/decoration/ter_mur/
scripts/custom/worldgen/decoration/tokuno/
scripts/custom/worldgen/decoration/trammel/



You may want to increase these settings in sphere.ini, here's how mine look

// Max NPC chars for a sector to prevent lag
MaxComplexity=128		//32

// Amount of items in one sector to start showing "x items too complex"
MaxSectorComplexity=2048		//1024


After that you're good to go just go in game add i_world_decorator and i_world_spawner

dclick the items then you can spawn and decorate your world. 

THANKS AND HAVE FUN!


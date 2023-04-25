# Breaking Down Walls - Teeth and Fortifications in Beyond All Reason
<sub></sup>(Author: TitanShadow12)</sup></sub>

Walls in Beyond All Reason are a cheap and simple way to shore up gaps in defenses or mess with enemy pathfinding. The width of most maps in BAR along with the slowness and risk of using constructors to build walls make these structures seem like a very niche form of passive defense, but with some cleverness and proper placement, even the tiny Dragon's Teeth can make an impact on your frontline.

## Wall Stats
The following 3 walls will be covered in this guide.

### Dragon's Teeth (T1 Walls)
> stats here
Constructed By: x, y, z
### Shark's Teeth (T1 Naval Walls)
> stats here
Constructed By: x, y, z
### Fortification Walls (T2 Walls)
> stats here
Constructed By: x, y, z

## Wall Basics
Let's set some ground rules you'll find common among walls in Beyond All Reason before we get into strategies and technical bits.
- Walls obstruct pathfinding and unit movement
- Some units can crush walls in their path and do not have their pathfinding interrupted
- Walls cost 0 energy and a small amount of metal
- Walls have extremely high HP for their cost
- Walls are built one unit at a time, and all walls have the same footprint size (verify for naval walls). Building walls by holding shift to place lines is much more effective than laying them down one at a time
- Walls do not block line of sight or affect targeting

## Walls Obstruct Movement


## Naval Walls - Shorelines???

## Best Wall Constructors
> cover each con and how well they place walls



# UNCATEGORIZED
Single layer walls:
0space walls stop everything
1space walls stop everything, but small units can get squeezed past the walls. They won't path through them, but you can try and shimmy small units through. E.g. grunts, incisors. Light tanks work well because they have a large turn radius, so it takes them a while to try and path around which causes them to collide and squeeze through.
2space *can* stop medium tanks (unreliable, sometimes they slip through at a diagonal) and T1 arty. Tanks will try to path around 2 spaced walls but can slip through if the angle is right.

Double layer walls:
Staggering spacing improves wall effectiveness.
0space walls need 3 segments destroyed to allow units to pass through. In practice this ends up being more due to units destroying walls to get to the segments behind.
1space and 2space walls don't get any improvements with passthrough, but do change the angle required for focus fire.

Walls can block damage from some units. This depends on angle and proximity. Grunts and pawns that rush an LLT protected by walls will find many shots hitting the walls instead once they close the distance. Using fight-move helps against this, but pawns will have more shots miss due to this. An LLT on a ramp with walls in front is much more resistant to grunts/pawns until the walls break (remember 2.8k hp each for 8 metal)
This also protects vs blitz/incisor, but is useless vs medium tanks, plasma bots, and missile trucks. Artillery also doesn't care.


But what's the *real* way to protect your LLTs from pawns/grunts? Walls further away.
You'll want to use 0 spacing on these walls to prevent shots between the walls getting through.
Wall Spaces Away	Pawn Results			Grunt Results
0					Minor damage blocked	No damage blocked except at rare angles
1					Minor damage blocked	Damage blocked at some angles
2					Most damage blocked		Damage blocked at most angles
3					All damage blocked		Damage blocked at all angles
4					Out of range			Damage blocked at all angles
5					Out of range			90% of time out of range
6					Out of range			Out of range
As you can see, walls directly in front of the LLT are ineffective at blocking damage on flat ground.
At 2 wall segments of distance away, the walls start paying dividends, and at 3 wall segments away your LLT is almost immune.
5 wall segments away is the sweet spot that forces your opponent to target the walls manually to make any progress, all while in range of the LLT.
At 6 walls away, grunts can just barely shoot the walls to make a hole while not in range of the LLT.
Don't even bother using walls against plasma bots, rocket bots, centurions, or medium tanks to protect LLTs.
3 wall segments happens to be the max range for commander build, but you probably don't have time to encircle yourself in walls before the raiders close in.

You can remove your own walls with self-d. All walls (yours and opponents) can be reclaimed very quickly.

Confusing pathfinding using singular gaps

Popup turrets on holdfire, stealth and what it looks like, destroyed popups, jammed walls

Ticks can't shoot over
Some units are short enough to be fully protected by walls against raiders and rockets. This includes:
most T1 units, including plasma bots
T1 labs
metal extractors (12 walls or 96m to surround), including exploiters (at longer ranges vs rockets)
construction turrets
solar panels
advanced solar panels
wind generators (suprisingly)
popup turrets (don't forget to rotate towards enemy)
--What looks like a bug: Arm T2 popup (Pitbull) won't pop up if there's walls in front, but if you force fire it to popup then give it a stop order it'll have no problems shooting enemies. Cor T2 popup doesn't have this issue.
commander (not vs rockets, can retaliate vs raiders)
--I leave T2 as an exercise for the reader
--Don't count on this against units with arcing shots.

Need a rocket bot or missile truck counter? They struggle to shoot over walls, so just build diagonally towards your enemy.
Fight over your walls using plasma bots or tanks.
Rocket bots / missile trucks shoot higher against LLTs, so again don't use walls to protect LLTs against rockets.

Remember, you can't repair walls. Reclaim and rebuild.

Use Ctrl+Shift to fully surround a building with walls.
When using minelayers, hold shift+space when queuing up walls and mines so they split up the task (they can't assist each other)

Alternative Walls
Solar panels aren't glamorous, but at least they don't die if you breathe on them too hard. In your own base, use solars to protect your base LLT.
Wind turbines will OBSTRUCT LLTs, but solars will not.
If you're quick enough, you can block attacks using a nanoframe (the building under construction).

T2 tanks and T3 units can walk over walls, taking some damage (about 250 per wall).
Fortification walls can also be trampled by some T3 units. (which ones??)
Based on crushstrength in movedef
252: BOAT7, BOAT8, HHOVER4, HTANK4, HBOT3, HBOT4, HABOT4, HABOT3, HTBOT4
250: MTANK3, HTANK3,
1400: HTANK5, VBOT3, VBOT5, HBOT5
some chickens and scavs can also crush walls

Fortification Walls
These block direct fire along with hounds and sheldons.
They won't protect you from T2 missile artillery (T2 vehicle and T2 Cor bot Arbiter)
The tall turrets can all fire over these, including Bulwark and Pulsar along with LLT, DLLT, and Beamer (the last two are notably in the combat engineers' build lists)
They do not block radar, jamming, or LoS.
T2 static artillery on High Trajectory mode can fire over these, and so can tactical missiles.
Use these to bolster the HP of your pulsars, bulwarks, and radars, and consider using them to help hold ground against Sheldon pushes or similar.

all that glitters replay (started West side) prior to april 25

/debugcolvol to see targeting.

mention footprint size
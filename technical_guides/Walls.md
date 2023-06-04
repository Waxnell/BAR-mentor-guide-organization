# Breaking Down Walls - Teeth and Fortifications in Beyond All Reason
<sub></sup>(Author: TitanShadow12)</sup></sub>

Walls in Beyond All Reason are a cheap and simple way to shore up gaps in defenses or mess with enemy pathfinding. The width of most maps in BAR along with the slowness and risk of using constructors to build walls make these structures seem like a very niche form of passive defense, but with some cleverness and proper placement, even the tiny Dragon's Teeth can make an impact on your frontline.

## Wall Stats
The following 3 walls will be covered in this guide.


| Name | Unitdefname | HP | Regen | Metal Cost | Energy Cost | Buildtime | Constructed By |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **Dragon's Teeth (T1 Walls)** | armdrag / cordrag | 2800 | 4/s | 8 | 0 | 255 | All T1 cons, minelayers, commanders |
| **Shark's Teeth (T1 Naval Walls)** | armfdrag / corfdrag | 4450 | 4/s | 15 | 0 | 400 | T1 vehicle amphib, hover, seaplane, and ship cons; commanders |
| **Fortification Walls (T2 Walls)** | armfort / corfort | 8900 | 12/s | 40 | 500 | 900 | All T2 constructors (except ship), Twitcher, Consul |

## Wall Basics
Let's set some ground rules you'll find common among walls in Beyond All Reason before we get into strategies and technical bits.
- Walls obstruct pathfinding and unit movement
- Some units can crush walls in their path and do not have their pathfinding interrupted
- Walls cost 0 energy and a small amount of metal
- Walls have extremely high HP for their cost
- Walls are built one unit at a time, and all walls have the same footprint size (verify for naval walls). Building walls by holding shift to place lines is much more effective than laying them down one at a time
- Walls do not block line of sight or affect targeting
- Walls are not discovered by radar, only line of sight will reveal them; however, once revealed, their location will persist in the fog of war.
- Walls can be captured, but reclaiming them is faster and they provide no line of sight, so this doesn't serve a purpose.
- Walls cannot be repaired
- Walls have a footprint of 2x2, which is bigger than the footprint of Perimeter Cameras (1x1)

![Footprint](https://i.imgur.com/bgNgRfz.png)

### T1 Popup Turrets

T1 Popups share several similarities with walls
- T1 Popup turrets are mostly indistinguishable from walls while closed
- Setting a T1 Popup to Hold Fire can hide it almost completely from the enemy until the right moment to strike  

## Walls Obstruct Movement

The most obvious use of walls is to obstruct unit movement and pathfinding.
- Adjacent walls block unit movement
- Hold shift and alt and tap z or x to increase or decrease unit spacing.
    - Walls with 1 unit spacing (half a wall segment) will still block all units, giving more length for the same cost.
    - Walls with 2 unit spacing (a full wall segment) will not block most units, but will block some bigger units (e.g. medium tanks and artillery)
- Some units are barely small enough to fit through walls, but will not pathfind through them. This includes pawns/grunts through singly spaced walls and medium tanks through double spaced walls. Ramming a blob of units or abusing their turn rate may result in "leaks," where a few units get pushed through the wall. Leaks will not happen through adjacent walls.

![Wall Spacing](https://i.imgur.com/UF96gSh.png)

- Sharks teeth will block land units on shallow water, and will also block submarines in shallow water. In deep water, submarines can move underneath the sharks teeth. 
- Sharks teeth require even less spacing to block units.
    - Nothing will path or leak throu 1 space walls
    - Corvettes and scout boats (small boats) will leak through 2 space walls
    - Small boats and submarines (when applicable) can path through 3 space walls, while bigger boats (frigates and destroyers) can leak.
    - 4 space walls are fine for all T1 boats
    - 5 space walls are passable by even T2 boats, if they don't crush them.

![Naval Wall Spacing](https://i.imgur.com/Im7CWPL.png)

### Double layer walls
Staggering spacing improves wall effectiveness.
0space walls need 3 segments destroyed to allow units to pass through. In practice this ends up being more due to units destroying walls to get to the segments behind.
1space and 2space walls don't get any improvements with passthrough, but do change the angle required for focus fire.

### Disrupting Pathfinding
- Units will path right through walls they can crush (even friendly ones), so be aware of that if you start building tanks or T3 (i.e., reclaim or self-d your walls).
- Though units can squeeze through pretty small gaps in walls, units will still clump up around these gaps if too many try to move through at once, especially if those units are using line move with a slow turn rate.
- Jammed enemy walls and undiscovered walls are not taken into account for unit pathfinding until they are in vision range or discovered, respectively.
- Units will pathfind around walls to find the shortest unobstructed path, even from a long distance. This means an inattentive player can send their units a completely different path if they command their units to move past the wall when it would otherwise be much better to approach (and eventually destroy) the wall. This is particularly noticable on lanes approaching bases, where players like to just right-click units deep into enemy lines.

## Destroying Walls
- Walls will not be automatically targeted by units. You can manually issue an attack order on walls in LoS, but not those only in radar range. You can attack-ground to destroy those walls, and the radar icon will disappear (but the ghost will remain).
- T1 Popup Turrets will also not be automatically targeted by units unless they are attacking. They are also indistinguishable from walls from the opponent's PoV, until attacking. Units that begin automatically attacking a T1 popup will stop attacking it once it retracts, even if on fight-move.
- You cannot view the health of enemy walls, but each wall segment model visually degrades, darkens, and warps as it takes damage.
- T1 Popup turrets take significantly reduced damage while closed (1/4th damage), which makes them very easy to repair and very resistant to artillery unless baited open, e.g. by a slow trickle of spam units.
### Crushing Walls
Of course, not all units will be stopped by walls.
Generally, larger units will path through walls and destroy them, taking some damage in the process.
Technically, each unit has a defined "movedef" with specific "crushstrength" which will destroy walls if it exceeds their "crushresistance." Walls have a death explosion with a small AoE, so the damage varies depending on the unit's position relative to the wall, but hovers somewhere around 250 for Dragon's Teeth and 500 for Shark's Teeth and Fortification Walls.

<details>

<summary>Units that crush Dragon's Teeth / Shark's Teeth</summary>

- Bull
- Tiger
- Banisher
- Tzar
- Tremor
- Starlight
- Negotiator
- Diplomat
- Cataphract
- Lunkhead
- Fatboy
- Mammoth
- Razorback
- Catapult
- Shiva
- Marauder
- Vanguard
- Karganeth
- Arm/Cor Battleships (Dreadnought, Despot)
- Arm/Cor Carriers (Haven, Oasis)
- Arm/Cor Flagships (Epoch, Black Hydra)
- All units that crush Fortification Walls

</details>

<details>

<summary>Units that crush Fortification Walls</summary>

- Thor
- Titan
- Juggernaut
- Behemoth
</details>

<details>

<summary>PvE Wall Crushers</summary>

All walls:

- Raptor Queen
- Epic Scavs
- Spectre Apex Brawler
- Apex Brawler

Small walls:

- Apex Paralyzer
- Apex Acid Spitter
- Main Assault Raptor
- Mortar (All Types)
- All-Terrain Brawler (All Types)

</details>

## Building Lots of Walls
Placing walls individually is time consuming. Remember the following shortcuts:
- C > C to select walls (on grid hotkeys). For minelayers and naval constructors, this is C > X instead. Commanders build naval walls using C > S.
- Hold shift and left click and drag to place a line of walls.
- Hold shift and alt to place a box of walls.
- Tap Z and X while holding shift and alt to change wall spacing.
- With walls selected, hold ctrl and shift and click on an existing structure or ghost structure to surround it with walls (0 spacing). *This is particularly useful for surrounding T1 popup turrets.*
- Hold shift+space when assigning builders to place multiple walls so they split up the task equally among them, saving on walking time. *This is especially important for minelayers, as they cannot assist each other in construction.*

## Naval Walls and Shorelines
Naval walls can be placed in shallow or deep water, and land walls must be placed on dry land. On some shorelines, neither land nor sea walls can be placed. This can create problematic, irreparable gaps in walls where bots can path through the shallows.

![Shoreline Walls](https://i.imgur.com/mKLQWjP.png)

Submarines and amphibious units can ignore naval walls by going under them. However, in shallow water the naval wall's collider extends deep enough that submarines cannot submerge low enough to pass underneath, effectively blocking them.

![Submarines Blocked by Walls](https://i.imgur.com/cIOCJNX.png)

## Best Wall Constructors
| Unit Type | Pros | Cons |
| --- | --- | --- |
| Commander | VERY useful on front line, high buildpower | Usually want to build LLTs, disaster if ambushed |
| T1 Cons | Useful on front line, can build popups | Slow, vulnerable, expensive |
| Minelayers | Can also build mines, cheap, fast, has local jamming | Cannot support each other, restricted to T1 vehicle lab |
| T2 Cons | Can build highest tier T2 defenses that synergize with fortress walls | Expensive, vulnerable, slow |
| Combat Engineers | Can build tall T2 defenses that syndergize with fortress walls, fast, good for reclaim as well, build mines | Restricted to specific T2 labs |

- Minelayers are ideal for building T1 walls, and combat engineers are ideal for building T2 walls. However, these are specific to certain factories. Arm bot players will see neither of these options.
- In the early game, the commander can quickly build a bunker for artillery or plasma to fight vs rocket bots
## Walls as Protection / Cover
Walls can block damage from some units against some units. Technically, whether a weapon will be blocked by a wall depends on whether the projectile's path from the weapon to the target's "aimposition" will be blocked by the wall's collision volume. In layman's terms, this means some units (usually ones lower to the ground) will be easier to protect with walls, and some units (usually ones with arcing shots, e.g. plasma bots) will be harder or impossible to defend against using walls. 

![Walled Arty](https://i.imgur.com/txonxoj.gif)

You can use the /debugcolvol command to view target collision. There will be a dot indicating the aimposition, which is where enemies will aim to destroy the unit. For most T1 units (including windmills, oddly enough), this is close to the ground and about level with Dragon's Teeth, so they'll be safe vs direct fire weapons behind walls. In T1 this includes all scout and raider units as well as missile trucks, rocket bots, and Centurions.

![Debugcolvol](https://i.imgur.com/lMiB7cF.png)

![Debugcolvol lineup](https://i.imgur.com/0SxcDTX.png)

- Constructors will be safe from rocket bots and pawns/grunts when behind walls, allowing you to build popup turrets, or more walls
- *This is especially powerful for T1 popup turrets (Dragon's Claw / Maw), which are not only disguised as walls but easily protected by them as well.*
- ![Walled Popup](https://i.imgur.com/jvT0d2E.gif)
  - Side note on T1 popup turrets: make sure you set the T1 popup turrets building facing towards the enemy so they extend to fire and retract much more quickly. T2 popup turrets preserve their facing.

<details>

<summary>Note on T2 popup turrets</summary>

T2 popup turrets are also protected by T1 walls, but there is a bit of unintended behavior with Pitbulls (Arm T2 popup). If there is a wall adjacent to it and between it and its target, it will not pop up to fire. If it is already popped up (e.g. from firing beforehand), it will fire on units in range. Keep this in mind if you choose to protect pitbulls with walls.

</details>

Don't bother trying to block your enemy's plasma bots, medium tanks, or artillery; in fact, consider parking your plasma bots behind walls to siege against a rocket bot or missile truck spammer.

- *Build diagonally towards the enemy!*

Commanders and most tall defense towers (e.g. LLT) have a higher aimposition. This means most units will have little trouble shooting at them, even if a wall is right in front of the tower.

So are walls useless at protecting LLTs? Not so! There is another way to force the wall in the projectiles path: build the wall further from the tower. Pawns / grunts adjacent to walls have trouble shooting at anything on the other side because their guns are basically right up against the wall, despite being angled upward. 

You'll want to use 0 spacing on these walls to prevent shots going through gaps in the wall.

| Wall Spaces Away	| Pawn Results			| Grunt Results |
| ----------------- | --------------------- | ------------- |
| 0					| Minor damage blocked	| No damage blocked except at rare angles |
| 1					| Minor damage blocked	| Damage blocked at some angles |
| 2					| Most damage blocked	| Damage blocked at most angles |
| 3					| All damage blocked	| Damage blocked at all angles |
| 4					| Out of range			| Damage blocked at all angles |
| 5					| Out of range			| 90% of time out of range |
| 6					| Out of range			| Out of range |

As you can see, walls directly in front of the LLT are ineffective at blocking damage on flat ground.
- At 2 wall segments of distance away, the walls start paying dividends
- At 3 wall segments away your LLT is almost immune.
- At 5 wall segments away is the sweet spot that forces your opponent to target the walls manually to make any progress, all while in range of the LLT.
- At 6 walls away, grunts can just barely shoot the walls to make a hole while not in range of the LLT.

Here's an image to show what I mean, with decreasing spacing from left to right (LLT set to hold fire):

![Protecting LLT with Walls 2](https://i.imgur.com/LeBKVR4.png)

The rightmost LLTs get destroyed much more quickly, while the leftmost LLTs don't even draw fire. The furthest left LLT (6 segments) cannot target the grunt in the back that is shooting the wall (just out of range)

Note, however, that rocket bots and missile trucks have plenty of range to allow projectiles to gain height and hit your towers. 

Terrain can also make your walls more effective as cover. An LLT higher on a ramp with walls in front is much more resistant to raiders until the walls break. On a steep enough ramp, these walls can be placed directly in front of the tower (0 spacing) and still prove effective.

![Walls on Ramps](https://i.imgur.com/AhHLJ3Y.png)

20 pawns normally would stomp three LLTs, but with walls it's a slightly different story:

![Walls on Ramps Outcome](https://imgur.com/T5EDjvH.png)

With walls, the pawn force is severely weakened. Without the walls there, pawns take only marginal losses:

![No Walls on Ramps Outcome](https://i.imgur.com/ej7PCtj.png)

Walls don't work so well against opponents attacking from uphill:

![Walls on Ramps Uphill Outcome](https://i.imgur.com/lKJBNm3.png)

### Note on Shark's Teeth / Naval Walls - The Submarine Bunker

Shark's Teeth collision extends low enough to block torpedos from enemy submarines. However, torpedos from your own submarines and depth charges from your destroyers will NOT be blocked by your walls. Your walls will block your opponent's depth charges and torpedos against subs, but probably not vs units on the ocean floor (this depends on the angle of attack). Torpedo turrets will not fire through your walls, and neither will the floating HLT.
Many T1 ships can be protected by letting them hug walls, but it's a tossup on whether they'll be able to shoot back or not.

![Submarine Bunker](https://i.imgur.com/Ut9cMDb.png)

2 Arm T1 subs against 4 destroyers? And only 240 metal of walls?

![Submarine Bunker 2](https://i.imgur.com/wo4QlMt.png)

Might be the best T1 sea static defense in the game.

## Cleaning Up Walls
Walls can be reclaimed almost instanteneously, refunding their full metal cost. This is much faster than destroying them, so if you come across enemy walls in your way try to reclaim them using an engineer, rezbot, or your commander. They're not worth much, so only do this if it'll help your strategic position or if there are a lot of easy-to-access walls.

Remember, you can't repair walls. Reclaim and rebuild.

Your opponent may try to turn your own walls against you. While you can reclaim your own walls, you can also self-destruct them if you're in a hurry (e.g. if an enemy has pushed plasma bots onto your fortifications).

## Fortification Walls

T2 Fortification Walls are simply taller and tougher Dragon's Teeth. Their additional height means they block direct fire weapons along with low arcing shots, like those from hounds and sheldons, with a few catches:
- Splash damage still works through walls
- They won't protect you from T2 missile artillery (T2 vehicle and T2 Cor bot Arbiter)
- The tall turrets can all fire over these, including Bulwark and Pulsar along with LLT, DLLT, and Beamer (the last two are notably in the combat engineers' build lists)
    - T2 static artillery on High Trajectory mode can fire over these, and so can tactical missiles.
    - However, they are too tall for popup turrets and most units to shoot over
- They do not block radar, jamming, or LoS.

Use these to bolster the HP of your pulsars, bulwarks, and radars, and consider using them to help hold ground against Sheldon pushes or similar.
You can also use them to stop T2 tank pushes, as they won't get crushed like T1 walls will.

## Walls and Cloaking
Dragon's Teeth and Fortification Walls do not disrupt cloaking. Spybots, gremlins, etc. can pass near the walls without losing their cloaking effect.
T1 popup turrets (Dragon's Claw, Dragon's Maw) also do not disrupt cloak while they are disguised. Cloaked units in their vicinity will only be revealed while the turret is popped up, e.g. while attacking.

## Alternative "Walls"
The principles of defending your expensive stuff extend beyond the use of Dragon's Teeth.
- Solar panels aren't glamorous, but at least they don't die if you breathe on them too hard. In your own base, use solars to protect your base LLT.
    - Wind turbines will OBSTRUCT your LLTs, but solars will not.

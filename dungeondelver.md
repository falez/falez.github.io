---
layout: portfoliopage
title: Dungeon Delver
permalink: /portfolio/dungeondelver/index.html
---

![Dungeon Delver](/public/images/fypdungeondelver2.png)

<p class="message">
Dungeon Delver was my final year project when I was studying in MMU. I chose to create an Action RPG for Android tablet because I never made a mobile game, and I wanted to experiment with touch-based controls.
</p>

## About Dungeon Delver
Dungeon Delver is an "isometric-view" Action <strike>RPG</strike> game for Android tablet, made with Unity 3.5. The player character is a warrior, equipped with sword and shield, in a dungeon filled with skeletons and demons. The dungeon is composed of three levels, each with its own challenge.

###Controls
![Dungeon Delver](/public/images/fypdungeondelver3.png)

Movement: Left analog stick.

Attacking: Right side. Buttons. While attacking, the player stops moving and the analog stick is used for attack direction.

Healing: To consume potions, tap the HP or Energy bar.

The menu button on the top right will reveal more options to the player, such as character sheet.

###Enemies

There are 2 types of enemy in Dungeon Delver: normal and champion. Normal enemies only have basic attack (melee or ranged), while Champions have special attacks.

Normal enemies:

* Skeleton (melee)
* Earth Demon (melee)
* Skeleton Mage (ranged)
* Fire Demon (ranged)

Champions:

* Skeleton Knight - Summons minion, Shield Bash
* Golem - Spike, Ground Stomp
* Greater Demon - Spike, Ground Slam

#### AI

The enemy AI is state-based. Enemies have 2 states: Idle and Attacking.

Idle state:

In idle state, the enemy stands on guard. This is the default state of all enemies.

Enemies will enter Attacking state if the two conditions are met:
* The player is within aggro range.
* The enemy has direct line of sight on the player.

Attacking state:

In attacking state, the enemy will start moving towards the player if they are not within attack range. Enemies within range will start attacking the player and will chase the player if the player runs away.

Enemies in Attacking state will revert to Idle state if the two conditions are met:
* The player is outside its aggro range.
* The enemy lost sight of the player for 2 seconds.

On entering Idle state, the enemy will move back to its original location.


###Dungeon

####First Level
First level is an event-based level. The player needs to activate an altar to open a door. Skeletons will spawn on activating the altar. The door unlocks after the player kill the skeletons.

Beyond the door is a staircase that leads deeper to the dungeon, where Fire Demons and Earth Demons resides. At the end of the first level is a portal guarded by a Skeleton Knight. The portal stabilizes after the Skeleton Knight is killed, and the player can continue to the next level.

####Second Level
The second level is an item collection level. The player enters a room with two altars and a locked door. The player is required to collect two gemstones to unlock the door. The first gemstone is guarded by traps, while the second gemstone is guarded by an Ice Golem. After the door is unlocked the player continues to the next level.

####Third Level
The third level is a boss arena, where the player meets the Greater Demon. The objective is simply to kill the Greater Demon and enter the portal, where the player is greeted with a victory screen.

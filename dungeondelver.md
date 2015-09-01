---
layout: portfoliopage
title: Dungeon Delver
permalink: /portfolio/dungeondelver/index.html
---

![Dungeon Delver](/public/images/fypdungeondelver2.png)

<p class="message">
This project was my final year project. I chose to create a game for Android because I never made a mobile game before, and I wanted to experiment with touch-based controls.
</p>

## About Dungeon Delver
<hr class="h2line">
Dungeon Delver is an "isometric-view" Action RPG for Android tablet made with Unity 3.5. The player character is a warrior in a dungeon filled with skeletons and demons. The dungeon is composed of three levels, each with its own challenge.
<br><br>

##Player
<hr class="h2line">
The player character is a warrior equipped with sword and shield. The warrior has two skills:

* **Shield Bash:** Knock back an enemy and stun it for a few seconds.
* **Throw Dagger:** Throw a dagger that deals moderate damage. The warrior's only ranged attack.

The warrior has three attributes:

* **Strength:** Increases damage output.
* **Vitality:** Increase maximum health.
* **Endurance:** Increase maximum energy.

At level 1, the warrior has 5 points in each attribute. On leveling up, the player will receive 5 attribute points to spend on whichever attribute they prefer. The warrior can increase in level up to level 10.
<br><br>

##Controls
<hr class="h2line">
![Dungeon Delver](/public/images/fypdungeondelver3.png)

**Left Analog Stick:** Movement and attack direction<sup>1</sup>.<br>
**Red button:** Normal attack.<br>
**Shield button:** Shield Bash skill.<br>
**Dagger button:** Throw Dagger skill.<br>
**Health/Energy bar:** Recover Health/Energy. Consumes a potion.<br>
**Menu button:** Character attributes screen and options.

<sup>1</sup> *While attacking, the player stops moving and the analog stick is used for attack direction instead.*
<br><br>

##Enemies
<hr class="h2line">
There are two types of enemy in Dungeon Delver: normal and champion. Normal enemies only have basic attack, while Champions have special attacks. The player is rewarded with experience points on killing enemies.

Normal enemies:

* Skeleton (melee)
* Earth Demon (melee)
* Skeleton Mage (ranged)
* Fire Demon (ranged)

Champions:

* Skeleton Knight - Summons minion, Shield Bash
* Golem - Spike, Ground Stomp
* Greater Demon - Spike, Ground Slam
<br><br>

## AI
<hr class="h2line">
Enemies in Dungeon Delver uses a state-based AI. There are two states: Idle and Attacking.
<br>

###Idle
Idle state is the default state of all enemies. In this state, the enemy stands on guard and only checks if the player enters its aggro zone (a sphere-shaped trigger).

An enemy will transition into Attacking state if the two conditions are met:

1. The player is within aggro range.
2. The enemy has direct line of sight on the player.
<br>


###Attacking

In this state, the enemy will start moving towards the player until it reaches its attacking range. Once within range, it will start attacking the player. Enemies in Attacking state will chase the player if the player runs away.

Enemies in Attacking state will transition into Idle state if the two conditions are met:

1. The player is outside its aggro range.
2. The enemy lost sight of the player for at least 2 seconds.

On entering Idle state, the enemy will attempt to move back to its original location.
<br><br>

##Dungeon
<hr class="h2line">

###First Level
The first level is an event-based level. The player is required to activate an altar to unlock a door. However, skeletons will spawn on activating the altar. The door unlocks after the skeletons are dead.

Beyond the door is a staircase that leads deeper to the dungeon, where Fire Demons and Earth Demons resides. The player is introduced to checkpoints that act as respawn location.

At the end of the first level is a portal guarded by a Skeleton Knight and its minions. The portal stabilizes after the Skeleton Knight is defeated, and the player can enter the portal to continue to the next level.

###Second Level
The second level is an item collection level. The player reaches a hall with two empty pedestals and a locked door. The player is required to collect two gemstones; the first gemstone is guarded by series of traps, while the second gemstone is guarded by an Ice Golem. After placing both gemstones on each pedestal, the door unlocks and the player continues to the third level.

###Third Level
The third level is a boss fight. The player enters an arena and meets the Greater Demon. The objective is to eliminate the Greater Demon and enter the portal, where the player is greeted with a victory screen.
<p class="message">
Dungeon Delver's characters are obtained from Unity Asset Store.
</p>

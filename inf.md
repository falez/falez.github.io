---
layout: portfoliopage
title: INF
permalink: /portfolio/inf/index.html
---

![INF](/public/images/inf-2.png)

<p class="message">
This was my first Unity-based project, made because I was curious about Unity. I rewrote several AngryBots scripts from UnityScript to C# in order to learn about Unity's workflow. Unity also has an excellent documentation that made learning even easier. After INF, I decided to use Unity in my <a href="/portfolio/dungeondelver">final year project</a>.
</p>

## About INF
INF is a wave-based top-down shooter made with Unity 3.5 (scripted with C#) and uses AngryBots' player components as base. The player character is a marine located in an abandoned parking lot and faces waves of zombies. Bounties are rewarded on killing zombies, which is used to purchase upgrades and unlock new weapons. The player can access the shop at any time during gameplay.

In the beginning of the game, a wave is composed of small amount of slow-moving zombies. As the wave goes on, the amount of zombies increases and fast zombies start to appear. Fast zombie rewards higher bounty.

##The Player
The player starts with 100 Health and is equipped with an assault rifle. The player has three upgrades that increases survivability against the zombie horde.

**Upgrades:**

* Upgrade Health: Increase maximum health.
* Upgrade Armor: Mitigates damage from zombies.
* Regeneration: Enables Health regeneration.

##Player Arsenal
The player has access to three types of weapon. In the beginning, only the assault rifle is available to the player. The other two weapons, the shotgun and the flamethrower, can be unlocked by spending bounties. Each weapon can be upgraded and sports a unique reload mechanic.

###Assault Rifle
The assault rifle is a rapid fire weapon that deals moderate damage. The accuracy deteriorates each time a shot is fired and recovers over time. The assault rifle reload mechanic is magazine replacement, which refills ammo to full magazine size.

**Upgrades:**

* +MAG II/III/IV: Increases magazine size.
* +DAM II/III/IV: Increases the damage per bullet.
* +REL II/III/IV: Increases reload speed.
* Laser Sight: Increases accuracy and reduces accuracy deterioration.

###Shotgun
The shotgun is a slow firing weapon that fires 8 pellets per shot. The accuracy deteriorates each time a shot is fired and recovers over time. The shotgun reload mechanic is slug reloading, which refills ammo one by one.

**Upgrades:**

* +MAG II/III/IV: Increases magazine size.
* +DAM II/III/IV: Increases the damage per bullet.
* +RATE II/III/IV: Increases the rate of fire.
* Magazine Reload: Replaces slug reloading with magazine reloading.

###Flamethrower
The flamethrower is an area of effect weapon capable of burning enemies, dealing damage over time. The flamethrower has infinite ammo but cannot be fired indefinitely, as the weapon safety triggers when it gets too hot.

**Upgrades:**

* +DAM II/III/IV: Increases the damage per second.
* +RATE II/III/IV: Slows down the temperature gain.
* +BURN II/III/IV: Increases burning damage.
* Vent: Reloading decreases the weapon cool down.

<p class="message">
INF uses the player model from AngryBots, zombie model by PixelHouse and soldier model from Unity 3 sample project.
</p>

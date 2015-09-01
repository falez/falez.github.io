---
layout: portfoliopage
title: Troika
permalink: /portfolio/troika/index.html
---

![Troika](/public/images/troika2.png)

An endless, top down vehicular shooter made with XNA and FarseerPhysics. The player controls a vehicle and is surrounded by an endless wave of enemies. Score is rewarded upon enemy deaths (by shooting or ramming), and enemies have a chance to drop power-ups when killed. The game ends when the player dies.

The vehicle movement is driven by physics. Force is applied to the front tires which in turn pulls the chassis and the back tires. Collision between player, projectile and enemy is also handled using physics.

##Player
<hr class="h2line">
The player vehicle is equipped with three weapons:

* **Cannon:** A very accurate and high damaging weapon, but low fire rate.
* **Tri-Plasma:** Shoots three plasma in an arc that deals moderate damage and inaccurate at long range.
* **Machine Gun:** A rapid firing weapon but is very inaccurate and inflicts low damage.


##Enemies
<hr class="h2line">
The endless wave is composed of three types of enemies:

* **Fodder:** A weak and slow moving enemy.
* **Chaser:** A weak and slow moving enemy, but will charge towards the player if the player is too close.
* **Interval:** A strong enemy, but only moves in an interval.

##Power Ups
<hr class="h2line">
Enemies have a chance to drop power-ups upon death:

* **Reinforce Armor:** Repairs the vehicle for 50HP (up to 200HP).
* **Attack Speed:** Increases attack speed of all weapons for 7.5 seconds.
* **Score Multiplier:** Doubles score gain by 200% for 7.5 seconds.
* **Time Slow:** Slows time but increases maneuverability and attack speed for 7.5 seconds.

##Notes
<hr class="h2line">
The original intention of using FarseerPhysics was to handle collisions because I had problems with it in a prior assignment. It was an overkill solution and brought more problems (handling collision responses and queuing for deletion) but at least the player vehicle movement is nicer and I learnt about game physics.

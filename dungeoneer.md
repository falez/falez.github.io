---
layout: portfoliopage
title: Dungeoneer
permalink: /portfolio/dungeoneer/index.html
---

![Dungeoneer](/public/images/dungeoneer2.png)

An endless, turn-based rogue-like game made with DirectX9. The player plays as a warrior in procedurally generated dungeons. The objective is to find the teleporter to go to the next dungeon floor while killing enemies and finding loot. The dungeon is generated using [Cellular Automata][CA] method (four iterations). The starting and exit point is then placed on the map, and finally enemies and chests are scattered around the map.

##Player
<hr class="h2line">
The warrior has 4 main attributes. The attributes can be increased permanently by leveling up (ten levels) and finding better equipment (nine tiers):

* **Hit Points (HP):** The hit points of the warrior. Dies if HP is zero.
* **Damage (DAM):** The raw damage the warrior deals before damage mitigation. Enhanced by equipping better swords.
* **Defense (DEF):** The damage reduction before hit points is reduced. Enhanced by equipping better armor.
* **Agility (AGI):** Dodge rating of the warrior. High agility makes the warrior harder to be hit by an enemy attack. Enhanced by equipping better boots.

The warrior carries four types of potions (maximum of five for each type): Healing potion and temporary attribute-boosters (+DAM, +DEF or +AGI for six turns).

##Dungeon
<hr class="h2line">
Each dungeon floor is populated with two enemy types: weak and strong enemy. Enemies grow stronger (+DAM and +DEF) and loot quality improves every two floors (up to tenth floor).

<p class="message">
Oryx's Lo-Fi Fantasy spritesheet and DokuCraft's Minecraft texture pack were used at the time of development.
</p>
[CA]: http://www.roguebasin.com/index.php?title=Cellular_Automata_Method_for_Generating_Random_Cave-Like_Levels

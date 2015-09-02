---
layout: portfoliopage
title: TacTicToe
permalink: /portfolio/tactictoe/index.html
---

![TacTicToe](/public/images/tactictoe2.png)

A two player TicTacToe game where inside each major TicTacToe cell is another TicTacToe instance. Made with SFML.

##Gameplay
<hr class="h2line">
At the start of the game, a random major TicTacToe cell (containing a minor TicTacToe instance) is selected. The currently moving player can only place his or her mark inside the selected TicTacToe instance. Once a mark is placed, the next major TicTacToe cell is selected based on the location of the mark that was placed.

The winning condition is to successfully place three markers in horizontal/vertical/diagonal row in a minor TicTacToe instance.

###Example:

* Player 1 move in Major2.
* Player 1 place marker in Major2Minor9.
* Player 2 move in Major9.
* Player 2 place marker in Major9Minor9.
* Player 1 move in Major9.
* Player 1 place marker in Major9Minor5.
* Player 2 move in Major5.

...and so on.

[Download (Windows)](https://dl.dropboxusercontent.com/u/7422512/TacTicToe.zip)

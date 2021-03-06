---
layout: post
title: Conway's Game of Life
subtitle: This is a recreation of Conway's Game of Life!
cover-img: /assets/img/gol_banner.png
thumbnail-img: https://media.giphy.com/media/l0EQk94CE5zNqyFPHx/giphy.gif
share-img: https://media.giphy.com/media/l0EQk94CE5zNqyFPHx/giphy.gif
tags: [Games]
comments: true
---

John Conway's 'Game of Life' is a program created in 1970 that simulates a cellular automation. For this project, I attempted to recreate this game. You can check out my recreation [here](https://github.com/brucebra000/cspt12-Build-Week-1).

<p align="center">
  <img src="https://media.giphy.com/media/l0EQk94CE5zNqyFPHx/giphy.gif" alt="Game of Life"/>
</p>

# What is John Conway's Game of Life?

John Conway's 'Game of Life' is a zero-player video game, meaning the player doesn't actually have any input beyond setting variables before the game starts. The game is a simulation of cellular automaton. The way it works is simple; chose which cells on a grid are alive or dead, then run the simulation to see how they change over time. The black cells are alive, the white cells are dead. For each generation, a cell will become alive or dead based on which states its neighboring cells are in. Its neighbors are the 8 cells surrounding it. The conditions are as follows:

- If a live cell has fewer than 2 live neighbors, it will die.
- If a live cell has exactly 2 or 3 live neighbors, it will survive.
- If a live cell has more than 3 live neighbors, it will die.
- If a dead cell has exactly 3 live neighbors, it will become alive.

Let's take a look at this example. Here, the top-middle, middle-left, and middle-right squares are alive.

<p align="center">
  <img src="https://raw.githubusercontent.com/brucebra000/brucebra000.github.io/master/assets/img/gol_ex1.png" alt="gol ex1"/>
</p>

So given the rules above, the middle-left and middle-right cells will die, since they only have 1 living neighbor. The top-middle cell survives this generation since it has 2 living neighbors. The cell in the middle has become alive since that cell was surrounded by exactly 3 live cells.

<p align="center">
  <img src="https://raw.githubusercontent.com/brucebra000/brucebra000.github.io/master/assets/img/gol_ex2.png" alt="gol ex2"/>
</p>

The right arangment of cells allow you to make some pretty cool things! Check out how this combination evolves over time:

<p align="center">
  <img src="https://media.giphy.com/media/5p6NeJiqeW9qfWgzBU/giphy.gif" alt="Cool pattern"/>
</p>

# Playing the Game

The github for the game can be found [here](https://github.com/brucebra000/cspt12-Build-Week-1). Once you've created an environment and installed the requirements, then you can run GoL.py to launch the game.

<p align="center">
  <img src="https://raw.githubusercontent.com/brucebra000/brucebra000.github.io/master/assets/img/gol_open.png" alt="Open the game"/>
</p>

Clicking on a cell will change the state of that cell.

<p align="center">
  <img src="https://raw.githubusercontent.com/brucebra000/brucebra000.github.io/master/assets/img/gol_grid.png" alt="Click the grid"/>
</p>

Pressing 'Random' will randomly assign which cells are alive.

<p align="center">
  <img src="https://raw.githubusercontent.com/brucebra000/brucebra000.github.io/master/assets/img/gol_random.png" alt="Random"/>
</p>

Pressing 'Next' will advance the generation by 1 stage.

<p align="center">
  <img src="https://raw.githubusercontent.com/brucebra000/brucebra000.github.io/master/assets/img/gol_next.png" alt="Next"/>
</p>

Pressing 'Start' will continuously advanced the generation by 1 stage. When this happens, the button will change to 'Stop', which will pause the simulation.

<p align="center">
  <img src="https://media.giphy.com/media/zgmA8Mfl7bx6EwiIqC/giphy.gif" alt="Start and Stop"/>
</p>

Changing the speed value will change how quickly the simulation will advance generations. This value can be adjusted from 1-60 with 30 being the default. A speed value of 60 is a full second between generations.

<p align="center">
  <img src="https://media.giphy.com/media/zFONt2IEnfkdG78hW4/giphy.gif" alt="Fast"/>
</p>

<p align="center">
  <img src="https://media.giphy.com/media/nXBjHNk4DiUS5Pg6BU/giphy.gif" alt="Slow"/>
</p>

Finally, clicking 'Clear' will remove all live cells from the grid and reset the generation back to 0.

<p align="center">
  <img src="https://raw.githubusercontent.com/brucebra000/brucebra000.github.io/master/assets/img/gol_open.png" alt="Slow"/>
</p>

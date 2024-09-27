+++
title = "Conway's Game of life implementation in Rust 🦀"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "A simple implementation of the conway's game of life written in rust."
tags = ['rust']
+++


## A simple implementation of the conway's game of life written in rust.

[`🐙 Github source here 🐙`](https://github.com/RealColorDream/game-of-life)

## Overview of the game

Conway's Game of Life is a cellular automaton devised by the British mathematician John Horton Conway in 1970. It is a zero-player game, meaning that its evolution is determined by its initial state, requiring no further input. The game consists of a grid of cells that can be either alive or dead, and it evolves through a series of generations based on a set of simple rules.

## Rules

The state of each cell in the grid is updated simultaneously based on the following rules:

1. **Survival**: A live cell with two or three live neighbors remains alive in the next generation.
2. **Death**: A live cell with fewer than two live neighbors dies (underpopulation), and a live cell with more than three live neighbors dies (overpopulation).
3. **Birth**: A dead cell with exactly three live neighbors becomes alive (reproduction).

These rules create a dynamic system where simple initial configurations can lead to complex behaviors over time.



### To Build and Run this project you need to have the following installed:

- Rust
- Cargo
- SDL2 (refer to the [guide of the embedded-graphics crate](https://docs.rs/embedded-graphics-simulator/0.6.0/embedded_graphics_simulator/#setup) for installation)


### The game is implemented using embedded-graphics and runs on a 64x64 monochrome display.

![](img/conways-Game-Of-Life.png)

#### Keybinds:
- `Space` to pause/unpause the game
- `TAB` to reset the game
- `Arrow keys` to move the cursor
- `Enter` to toggle the state of the cell under the cursor when the game is paused
- `Escape` to exit the game
- `LMB` to spawn a spaceship at the position of the cursor

Have fun!

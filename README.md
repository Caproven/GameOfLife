## Synopsis

This project is a simulation for [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life). The entire thing is written in Java, using the Swing/AWT libraries. The cell automation follows 4 simple rules:
1. Any live cell with fewer than two live neighbors dies, as if by under population.
2. Any live cell with two or three live neighbors lives on to the next generation.
3. Any live cell with more than three live neighbors dies, as if by over-population.
4. Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

## Motivation

I find cellular automata to be fascinating, and Conway's Game of Life seemed like a great starting point. I had seen the Game of Life before, but wanted to make my own implementation of it for practice with Java Swing. It is a rather simple simulation, but I decided that features could slowly be implemented, giving further experience with the software design cycle.

## Installation

The latest update can be found as an executable .jar in the GameOfLife/executables/ directory. Either double click it to run or enter "java -jar GoL.jar" into a console.

## Tests

Exclusively using the latest in hands-on debugging techniques (I spam click everything and see if it works).

## Updates

Version 0.7

Added
- Drawing system written from scratch. Previous implementation using JButtons was embarassing and I finally had some free time to mess around with new stuff. New implementation is significantly faster, but more benchmarking has to be done on better hardware than my laptop.
- Slider to change speed (tick rate)
- Resizability! Change size of grid along with cell size on the grid.

Fixed
- N/A

Other / Issues
- Compare potential differences between ConwayGUI.SimulationTicker extending Thread vs. implementing Runnable.
- Add more control over frames when opening Resize panel. Can currently use it to break things.

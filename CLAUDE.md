# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple Snake game implementation built with Phaser.js framework. The game runs entirely in the browser with no build process or external dependencies beyond the Phaser library.

## Architecture

- **Single-file application**: All game logic is contained in `index.html`
- **Phaser.js game framework**: Uses Phaser 3.x (via `phaser.min.js`)
- **No build system**: Direct HTML/JavaScript development
- **Asset loading**: Game sprites are loaded from external URLs (Phaser examples assets)

## Game Mechanics

- Snake movement controlled by arrow keys
- 16px grid-based movement system
- Food collection grows snake length
- Collision detection for walls
- Game over and restart functionality
- 800x600 game canvas with black background

## Development Workflow

- No build commands required - open `index.html` directly in browser
- No testing framework - manual testing via browser
- No linting/formatting tools configured
- Live reload not available - refresh browser after changes

## Key Functions

- `preload()`: Loads game assets from external URLs
- `create()`: Initializes game objects and event timers
- `moveSnake()`: Handles snake movement and collision logic
- `eatFood()`: Manages food consumption and snake growth
- `gameOver()`: Resets game state after collision

## External Dependencies

- Phaser.js (local `phaser.min.js` file)
- Game assets loaded from `https://phaser.io/examples/assets/snake/`
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Single-file web Tic Tac Toe game (`tictactoe.html`). No build step, no dependencies, no package manager.

## Development

Open in browser:
```
start tictactoe.html
```

## Architecture

Everything lives in `tictactoe.html` — HTML structure, CSS styles, and JavaScript logic are all inline.

**Game state** is managed with plain variables: `cells` (9-element array), `current` (active player), `over` (game ended), `vsCPU` (mode toggle), `scores` (persistent across restarts).

**CPU AI** uses minimax (`minimax()` + `bestMove()`) — the CPU plays as O and is unbeatable.

**Rendering** is full re-render on every move (`render()` rebuilds all 9 cell divs from scratch).

## Git & GitHub

Repository: `https://github.com/issubro69-creator/tictactoe`

Always commit and push after making changes. Use descriptive commit messages that explain *what* changed and *why*.

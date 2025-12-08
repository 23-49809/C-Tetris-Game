# C++ Tetris Game (raylib)

Modern Tetris clone written in C++17 with raylib 4.5. The repository includes a ready-to-run Windows build plus all assets for development.

## Features
- Classic seven-piece Tetris with rotation rollback on invalid moves
- Soft drop scoring and line clear bonuses
- Music and sound effects powered by raylib audio
- Lightweight codebase organized for tinkering or learning

## Controls
- `Left` / `Right`: move the active piece
- `Up`: rotate
- `Down`: soft drop (+1 point per cell)
- Any key after game over restarts the session

## Scoring
- 1 line: +100
- 2 lines: +300
- 3 lines: +500
- Soft drop: +1 per cell

## Running the bundled build (Windows)
- Launch `game.exe` from the repository root so it can locate `Sounds/`, `Font/`, and `lib/`.
- Do not move the executable without copying the asset folders alongside it.

## Prerequisites
- raylib 4.5+ development libraries
- C++17 compiler (e.g., MinGW-w64 on Windows or clang/gcc on macOS/Linux)
- `make` or `mingw32-make` in your PATH

## Build from source
1) Install the prerequisites above.
2) From the repository root, run `mingw32-make` (or `make`) to produce `game.exe` in the root directory.
3) Run the binary from the repository root to ensure assets load correctly.

## Repository layout
- `src/` gameplay logic, rendering, and input
- `Sounds/` music and effects
- `Font/` bitmap font
- `preview.jpg` screenshot
- `lib/` Windows runtime DLLs

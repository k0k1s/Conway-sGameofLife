# Rust + WASM: Conway's Game of Life

A high-performance implementation of John Conway's **Game of Life** built with **Rust** and compiled to **WebAssembly (WASM)**. This project demonstrates the power of Rust for heavy-computation tasks in the browser, providing smooth rendering and efficient state management.


## How it Works

The "universe" is represented as a flat array in Rust memory. 
- **Rust side:** Handles the logic for calculating the next generation of cells based on the standard rules (Birth, Survival, Overpopulation, Underpopulation).
- **JavaScript side:** Reads the shared memory buffer directly to render the cells onto an HTML5 `<canvas>` element, ensuring zero-copy overhead for maximum FPS.

## Rules of the Game

1.  Any live cell with fewer than two live neighbours dies (Underpopulation).
2.  Any live cell with two or three live neighbours lives on to the next generation.
3.  Any live cell with more than three live neighbours dies (Overpopulation).
4.  Any dead cell with exactly three live neighbours becomes a live cell (Reproduction).

## Created by 

Author - **k0k1s**, Using AI Gemini, Claude

Can view it through browser @ https://k0k1s.github.io/Conway-sGameofLife/
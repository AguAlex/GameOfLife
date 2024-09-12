# 🧬 Game of Life - x86 Assembly

This is an implementation of **Conway's Game of Life** in **x86 Assembly (AT&T syntax)**. The game runs in the terminal, simulating a cellular automaton where cells live, die, or multiply based on simple rules.

## 📜 Rules of the Game

The Game of Life is a grid-based simulation where each cell can be either **alive** (`1`) or **dead** (`0`). The game's evolution is determined by the following rules:

1. **Underpopulation**: A live cell with fewer than 2 live neighbors dies (cell becomes `0`).
2. **Overpopulation**: A live cell with more than 3 live neighbors dies (cell becomes `0`).
3. **Survival**: A live cell with 2 or 3 live neighbors survives to the next generation (remains `1`).
4. **Reproduction**: A dead cell with exactly 3 live neighbors becomes a live cell (cell becomes `1`).

Each generation is a step in the simulation, where these rules are applied to all cells in the grid simultaneously.

## ⚙️ Technologies Used

- **Assembly x86 (AT&T syntax)**: The game logic is implemented using assembly language for x86 architecture.
- **Terminal**: The game is designed to run entirely in the terminal/console.
- **ncurses** (optional): Can be used for rendering the grid in a more visually appealing way in some terminals.

## 🛠️ Run the Game

    Execute the compiled program in the terminal:

    ```bash
    ./GameOfLife
    ```

## 🎮 How to Play

- The game starts with an initial configuration of the grid, which can be manually set .
- The terminal will display the current state of the grid, where:
    - **`1`** represents a live cell 🟩
    - **`0`** represents a dead cell ⚫
- Each generation is computed based on the rules of the game, and the grid will update automatically.

## ✨ Features

- **Terminal-based simulation**: The game runs directly in the terminal, displaying the grid as a matrix of 1s and 0s.
- **Grid Update**: The grid updates in real time, showing the evolution of the cell population.
- **Optimized for x86 Assembly**: Efficient use of registers, memory access, and low-level operations to perform the simulation.

## 🤝 Contributing

Feel free to fork this repository, submit issues, or create pull requests with new features or optimizations. Contributions are always welcome!

## 🙌 Acknowledgments

- **John Conway**: For creating the fascinating **Game of Life**.
- **Assembly Community**: For helpful resources and guidance on x86 assembly.


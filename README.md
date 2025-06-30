# Maze Solver with Curses Interface

A Python-based maze representation and solver project showcasing an 8×20 grid (or configurable size) with a start (`O`) and exit (`X`). The maze features multiple twists, loops, and dead-ends to challenge path‑finding algorithms. This implementation uses BFS (Breadth‑First Search) to find the shortest path, visualized in the terminal with the `curses` library.

## Features

* **Configurable Maze Size:** Easily swap in different maze layouts by editing the `maze` variable or loading from an external file.
* **Terminal Visualization:** Real-time rendering of the maze and solver progress using `curses`.
* **Path‑Finding Algorithm:** Uses BFS to guarantee the shortest path in an unweighted grid.
* **Clear Markers:** Start marked with `O`, walls with `#`, open paths with spaces, and solution path with red `X` characters.

## Getting Started

### Prerequisites

* Python 3.6+
* Unix-like terminal (Linux, macOS) or Windows with compatible terminal emulator

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/maze-solver.git
   cd maze-solver
   ```

2. (Optional) Create and activate a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install any dependencies (if needed):

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Open `solver.py` (or your main script) and customize your maze:

   ```python
   maze = [
       ["#", "O", "#", ... ],
       [...],
       [...]
   ]
   ```

2. Run the solver:

   ```bash
   python solver.py
   ```

3. Watch the BFS algorithm explore and find the exit. Press any key to exit when the solution appears.

## Customization

* **Maze Layout:** Edit the `maze` list at the top of the script, or load layouts from a text file for greater flexibility.
* **Algorithm Variations:** Swap out the BFS implementation in `find_path` for DFS or A\* by evaluating neighbors differently and using a priority queue.
* **Visualization:** Tweak colors or display delays (`time.sleep`) in the `print_maze` function to change the look and speed.

## Contributing

Contributions are welcome! Feel free to open issues for bugs, feature requests, or enhancements. Fork the repo and submit a pull request with clear descriptions.


*Happy maze solving!*

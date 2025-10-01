# Pac-Man-Pathfinding-Simulator-

👾 Pac-Man in Maze World

📖 Background
Pac-Man is trapped in a haunted maze and needs to navigate safely to his destination while avoiding ghosts. The maze is represented as a 2D grid where:
0 → Empty cell (Pac-Man can move here)
1 → Ghost (blocked cell, Pac-Man cannot enter)

Your task is to build a navigation system for Pac-Man using only stacks.

⚙️ Features Implemented
🏰 Maze (maze.py)

Represents the maze as a 2D grid (list of lists).

Functions:

add_ghost(x, y) → Place a ghost at (x, y).
remove_ghost(x, y) → Remove ghost from (x, y).
is_ghost(x, y) → Check if (x, y) contains a ghost.
print_grid() → Print the maze layout in row-column format.

🧭 Navigator (navigator.py)
Implements Pac-Man’s navigation using stack-based DFS.

Function:

find_path(start, end)
Input: (s_x, s_y) → start coordinates, (e_x, e_y) → destination.
Output: A list of coordinates representing a valid path.

Raises PathNotFoundException if no valid path exists.

✅ Ensures:
Each cell is visited at most once.
Dead-ends are handled by backtracking using the stack.
Time complexity: O(n * m) for an n x m grid.

📦 Stack (stack.py)
Custom stack implementation (no built-in Python list stack methods).
Used for pathfinding and backtracking.

⚠️ Exceptions (exception.py)
Contains PathNotFoundException.
Raised when Pac-Man cannot reach the destination.

📂 File Structure
PacMan-Maze/
── maze.py         # Maze representation

── stack.py        # Custom stack implementation

── navigator.py    # Navigation system using stack

── exception.py    # Custom exception class

── main.py         # Testing & debugging file

── README.md       # Documentation (this file)

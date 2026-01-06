# A* Pathfinding Visualization 🔍

This project is a Python-based visualization of the **A* (A-Star) Pathfinding Algorithm**. It uses the `pygame` library to create an interactive grid where users can draw barriers, set start/end points, and watch the algorithm find the shortest path in real-time.



## 🛠️ Requirements

* Python 3.x
* Pygame

## 📦 Installation

1.  Clone the repository or download the script.
2.  Install the required library:
    ```bash
    pip install pygame
    ```
3.  Run the script:
    ```bash
    python a_star.py
    ```

## 🎮 Controls

| Interaction | Action |
| :--- | :--- |
| **Left Click** | **First click:** Set Start Node (Orange)<br>**Second click:** Set End Node (Turquoise)<br>**Subsequent clicks:** Draw Barriers (Black) |
| **Right Click** | Remove/Erase a node (Start, End, or Barrier) |
| **SPACE Bar** | Start the A* Algorithm |
| **C Key** | Clear the grid and restart |

## 🎨 Color Legend

* 🟧 **Orange:** Start Node
* Turquoise **Turquoise:** End Node
* ⬛ **Black:** Barrier (Wall)
* 🟩 **Green:** Open Set (Nodes being considered)
* 🟥 **Red:** Closed Set (Nodes already visited)
* 🟪 **Purple:** The Shortest Path (Final Result)

## 🧠 Algorithm Details

This implementation uses the **A* algorithm**, which combines:
1.  **G-Score:** The actual cost from the start node to the current node.
2.  **F-Score:** The estimated total cost (G-Score + Heuristic).

It utilizes **Euclidean Distance** as the heuristic function to calculate the distance between points, allowing for movement in 8 directions (including diagonals).

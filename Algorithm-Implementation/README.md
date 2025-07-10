# 🧠 Algorithm Implementations

Welcome to the **Algorithm-Implementation** repository! This repo contains a collection of fundamental AI and search algorithms, explained and implemented in an easy-to-understand format.

Each section below describes:
- 🛠 How the algorithm works  
- 📌 Where it is applied  
- ⏱ Time and space complexities  
- 🖼 Sample input/output visuals

---

## 📚 Table of Contents

- 🔍 [A-star](#a-star)
- 🎯 [Alpha-Beta Pruning](#alpha-beta-pruning)
- 🧮 [AO* Algorithm](#ao-star)
- 🌪 [Beam Search](#beam-search)
- 🧭 [Best First Search](#best-first-search)
- 🌉 [Breadth First Search (BFS)](#bfs)
- 🔄 [Bi-Directional Search](#bi-direction)
- 🌳 [Depth First Search (DFS)](#dfs)
- 🔥 [Depth Limited Search (DLS)](#dls)
- 🧠 [Iterative Deepening Search (IDP)](#idp)
- 🕹 [Min-Max Algorithm](#min-max)

---

<details>
<summary>🔍 <strong>A-star</strong></summary>

### 🛠 How It Works
A* is a best-first search algorithm that finds the least-cost path from a start node to a goal node using the formula:


```
f(n) = g(n) + h(n)

```

Where:
- `g(n)` = cost from the start node to current node  
- `h(n)` = estimated cost from current node to goal (heuristic)

### 📌 Applications
- GPS Navigation
- Game pathfinding
- Robot motion planning

### ⏱ Complexity
- Time: O(E)
- Space: O(V), where V is the number of vertices

### 🖼 Input & Output

![A-star Input](/images/a_star_input.png)  
![A-star Output](/images/a_star_output.png)

</details>

---

<details>
<summary>🎯 <strong>Alpha-Beta Pruning</strong></summary>

### 🛠 How It Works
An optimization technique for the Minimax algorithm that skips evaluating unnecessary nodes.

### 📌 Applications
- Game playing (Chess, Tic Tac Toe)
- AI decision making in adversarial environments

### ⏱ Complexity
- Time: O(b^d/2) with perfect ordering
- Space: O(bd)

### 🖼 Input & Output

![Alpha-Beta Input](/images/alpha_beta_input.png)  
![Alpha-Beta Output](/images/alpha_beta_output.png)

</details>

---

<details>
<summary>🧮 <strong>AO-star</strong></summary>

### 🛠 How It Works
AO* is a graph-based heuristic search for AND-OR graphs. It selects paths that minimize cost while considering all sub-goals.

### 📌 Applications
- Expert systems
- Automated planning

### ⏱ Complexity
- Time: Depends on graph structure (exponential in worst-case)
- Space: Proportional to nodes generated

### 🖼 Input & Output

![AO-star Input](/images/ao_star_input.png)  
![AO-star Output](/images/ao_star_output.png)

</details>

---

<details>
<summary>🌪 <strong>Beam Search</strong></summary>

### 🛠 How It Works
A variation of BFS that keeps only top-k nodes (beam width) at each level to reduce memory.

### 📌 Applications
- NLP decoding
- Speech recognition
- Chess AI

### ⏱ Complexity
- Time: O(bk)
- Space: O(k), where k = beam width

### 🖼 Input & Output

![Beam Search Input](/images/beam_input.png)  
![Beam Search Output](/images/beam_output.png)

</details>

---

<details>
<summary>🧭 <strong>Best First Search</strong></summary>

### 🛠 How It Works
Selects the most promising node based on a heuristic evaluation function.

### 📌 Applications
- Route planning
- Game AI
- Problem-solving

### ⏱ Complexity
- Time: O(n log n)
- Space: O(n)

### 🖼 Input & Output

![Best First Input](/images/best_first_input.png)  
![Best First Output](/images/best_first_output.png)

</details>

---

<details>
<summary>🌉 <strong>BFS (Breadth-First Search)</strong></summary>

### 🛠 How It Works
Explores all neighbors at current depth before going deeper.

### 📌 Applications
- Shortest path in unweighted graphs
- Crawlers
- Peer-to-peer networks

### ⏱ Complexity
- Time: O(V + E)
- Space: O(V)

### 🖼 Input & Output

![BFS Input](/images/bfs_input.png)  
![BFS Output](/images/bfs_output.png)

</details>

---

<details>
<summary>🔄 <strong>Bi-Directional Search</strong></summary>

### 🛠 How It Works
Runs two simultaneous searches—one forward from the start, and one backward from the goal.

### 📌 Applications
- Route finding
- Network routing

### ⏱ Complexity
- Time: O(b^(d/2))
- Space: O(b^(d/2))

### 🖼 Input & Output

![Bi-Directional Input](/images/bi_direction_input.png)  
![Bi-Directional Output](/images/bi_direction_output.png)

</details>

---

<details>
<summary>🌳 <strong>DFS (Depth-First Search)</strong></summary>

### 🛠 How It Works
Explores as far as possible along a branch before backtracking.

### 📌 Applications
- Topological sorting
- Solving mazes
- Cycle detection

### ⏱ Complexity
- Time: O(V + E)
- Space: O(V)

### 🖼 Input & Output

![DFS Input](/images/dfs_input.png)  
![DFS Output](/images/dfs_output.png)

</details>

---

<details>
<summary>🔥 <strong>DLS (Depth Limited Search)</strong></summary>

### 🛠 How It Works
A DFS with a predetermined depth limit to prevent infinite recursion.

### 📌 Applications
- When maximum depth is known
- Part of IDS

### ⏱ Complexity
- Time: O(b^l)
- Space: O(bl)

### 🖼 Input & Output

![DLS Input](/images/dls_input.png)  
![DLS Output](/images/dls_output.png)

</details>

---

<details>
<summary>🧠 <strong>IDP (Iterative Deepening)</strong></summary>

### 🛠 How It Works
Combines DFS and BFS by performing DFS repeatedly up to increasing depth limits.

### 📌 Applications
- Puzzle solving (e.g., 8-puzzle)
- Game trees

### ⏱ Complexity
- Time: O(b^d)
- Space: O(bd)

### 🖼 Input & Output

![IDP Input](/images/idp_input.png)  
![IDP Output](/images/idp_output.png)

</details>

---

<details>
<summary>🕹 <strong>Min-Max</strong></summary>

### 🛠 How It Works
Used in game theory; assumes both players play optimally to minimize/maximize score.

### 📌 Applications
- Chess AI
- Tic-Tac-Toe
- Strategic games

### ⏱ Complexity
- Time: O(b^d)
- Space: O(bd)

### 🖼 Input & Output

![Min-Max Input](/images/minmax_input.png)  
![Min-Max Output](/images/minmax_output.png)

</details>

---

## 🎨 Contribution & Usage

✅ Clone this repo  
🧠 Learn and explore the implementation  
📸 Replace placeholder images with actual visualizations from `/images`  
💬 Raise an issue or suggest improvements!

---

> 📌 _All implementations are written with clarity, documentation, and educational use in mind._  
> 📧 _Feel free to contribute or raise issues._

---

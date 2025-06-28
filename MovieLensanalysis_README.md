# MovieLens 2-Mode Network Analysis

This project analyzes the **MovieLens 100K** dataset as a **2-mode (bipartite) network** between users and movies. Using Python and NetworkX, we project the bipartite graph onto a user-user network, apply the **island method** to reduce complexity, and explore key patterns in user behavior.

---

## Dataset

- **Source:** [MovieLens 100K Dataset](https://grouplens.org/datasets/movielens/100k/)
- **Format:** User–Movie ratings with fields:
  - `user`, `movie`, `rating`, `timestamp`

---

## Methodology

### 1. Build Bipartite Graph
- Users and movies are nodes
- Edges connect users to movies they rated **≥ 3**

### 2. Project to User–User Graph
- Edges represent users who rated the same movie
- Edge weights = number of shared movies

### 3. Island Method
- Threshold: keep only edges with **≥ 10** shared movies
- Produces a dense subgraph of highly similar users

### 4. Community Detection (Label Propagation)
- Reveals grouping structure based on shared preferences

---

## Key Insights

- **Skewed degree distribution**: few highly connected users, many loosely connected
- **Island subgraph**: 953 users, 6,289 edges (dense core of similar users)
- **Top users**: The most connected users shared over 1,000 movies with others
- **Community structure**: One large community detected, suggesting broadly overlapping tastes

---

## Files

- `MovieLens_2Mode_Fixed.ipynb` – main notebook with all code, analysis, and visualizations
- `README.md` – this file

---

## Tools

- Python
- NetworkX
- Pandas
- Matplotlib

---

## Author

Ariba Razzak – CUNY SPS  
Course: DATA 620 – Social Network Analysis  


---

## How to Run

1. Download the [MovieLens 100K dataset](https://grouplens.org/datasets/movielens/100k/)
2. Place contents of `ml-100k/` in the same directory as the notebook
3. Open `MovieLens_2Mode_Fixed.ipynb` in Jupyter and run all cells

---

## License

This analysis is for educational use under fair use policy. Dataset © GroupLens Research.

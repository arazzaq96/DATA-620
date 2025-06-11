# Assignment 2: Graph Visualization

This assignment explores a real-world graph dataset using Python and NetworkX.

## Dataset
We used the `ca-GrQc.txt` collaboration network dataset from the Stanford SNAP collection:  
https://snap.stanford.edu/data/ca-GrQc.html

## Analysis Performed
The following metrics were computed:
- **Graph Diameter**: Longest shortest path between nodes
- **Average Clustering Coefficient**: Measures how connected neighbors are

To handle large sizes and improve analysis:
- The **largest connected component** was extracted
- **Self-loops** were removed for compatibility with metrics and layouts

## 🖼️ Visualization
We visualized a **k-core subgraph (k=5)** using `spring_layout` in NetworkX:
- This focused on a dense, interpretable subset of the graph
- Layout chosen for readability and spatial clustering

## Team
- [Ariba Mandavia]

## How to Run
This notebook uses Python 3 and requires:
- networkx
- matplotlib
- scipy


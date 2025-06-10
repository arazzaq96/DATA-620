# Assignment 3: Graph Visualization

This assignment explores a real-world graph dataset using Python and NetworkX.

## Dataset
We used the `ca-GrQc.txt` collaboration network dataset from the Stanford SNAP collection:  
https://snap.stanford.edu/data/ca-GrQc.html

## Analysis Performed
- **Graph Diameter**: Computed on the largest connected component
- **Average Clustering Coefficient**: To understand local connectivity

## Visualization
- We visualized a dense subgraph using a **k-core (k=5)** with `spring_layout`
- Self-loops were removed to avoid rendering and analysis errors
- Node size and layout were adjusted for clarity

## Team
- [Your Name(s)]

## How to Run
This notebook uses Python 3 and requires:
- networkx
- matplotlib
- scipy

Install requirements with:
```bash
pip install networkx matplotlib scipy

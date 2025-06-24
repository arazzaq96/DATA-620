
# Southern Women Network Analysis

This project analyzes the **Southern Women Dataset**, a classic bipartite network that captures the attendance of 18 women at 14 social events in a Southern U.S. town in 1930s. Originally studied in 1941, this small but rich dataset is frequently used to explore social network structures, centrality, and community formation.

---

## 📁 Dataset Description

- **Nodes**: 18 women + 14 events = 32 nodes
- **Edges**: Represent attendance (i.e., a woman attended a particular event)
- **Source**: Built-in `networkx.davis_southern_women_graph()` dataset

This is a **bipartite graph** consisting of two distinct node sets:
- Set 1: Women
- Set 2: Events

---

## 🎯 Objectives

- Explore and visualize the bipartite network of women and events
- Compute and compare centrality measures for both women and events
- Detect community structures among women
- Draw conclusions about social dynamics based on attendance patterns

---

## 🧪 Methods Used

- **Python Libraries**: `networkx`, `matplotlib`
- **Bipartite Graph Analysis**
- **Degree Centrality**
- **Projection onto single-mode network (Women-Women)**
- **Community Detection using Greedy Modularity**

---

## 📊 Key Findings

### Relationships between Women
- Women who attended the same events formed tightly connected clusters.
- Central women (e.g., Evelyn, Brenda) attended more events and acted as social bridges.
- Communities reflect social cliques based on shared event participation.

### Relationships between Events
- Events like E7, E8, and E9 were highly attended and served as key meeting points.
- Central events often brought together women from different clusters.

---

## 📁 Files

- `Southern_Women_Network_Analysis.ipynb`: Jupyter Notebook containing the full code, visualizations, and analysis
- `README.md`: This file

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. Install required packages:
   ```bash
   pip install networkx matplotlib
   ```

3. Run the notebook using Jupyter:
   ```bash
   jupyter notebook Southern_Women_Network_Analysis.ipynb
   ```

---

## 📚 References

- Davis, A., Gardner, B. B., & Gardner, M. R. (1941). *Deep South: A Social Anthropological Study of Caste and Class*.
- NetworkX documentation: https://networkx.github.io/documentation/stable/

---

## 👩‍💻 Author

**Ariba Mandavia**  
Graduate Student, CUNY SPS — Data Science  
Project Manager, Tech Incubator at Queens College  

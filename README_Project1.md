# DATA 620 – Project 1: Centrality Analysis by Categorical Group

## 👩‍💻 Author
Ariba Mandavia

## 📘 Project Overview
This project explores social network analysis using the **Zachary's Karate Club** dataset. The goal is to assess whether a node's **centrality** (degree and eigenvector) differs significantly by **club affiliation** (Mr. Hi vs Officer).

## 🧮 Methods
- Imported the dataset using NetworkX
- Calculated:
  - Degree Centrality
  - Eigenvector Centrality
- Grouped nodes by their `club` attribute
- Ran t-tests to compare centrality scores between groups
- Visualized results using boxplots

## 📊 Key Findings
- No statistically significant differences in centrality between club affiliations:
  - Degree Centrality: *p = 0.7953*
  - Eigenvector Centrality: *p = 0.7392*
- Slightly higher variability in Mr. Hi's group but not conclusive.

## 📦 Dependencies
- `networkx`
- `pandas`
- `matplotlib`
- `seaborn`
- `scipy`

## ▶️ How to Run
Open the notebook in Jupyter and run all cells. Ensure required packages are installed.

## 📁 Files
- `Project 1 Data 620.ipynb` – Main analysis notebook

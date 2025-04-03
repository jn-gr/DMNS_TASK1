# Email Network Analysis

This project analyses an email communication network from a research institution using network science techniques. The analysis focuses on understanding the structure and properties of the email communication patterns.

## Dataset

The analysis uses two main datasets:
1. `email-Eu-core.txt.gz`: Contains email communication links between members
2. `email-Eu-core-department-labels.txt.gz`: Contains department membership labels for each member
- Dataset from https://snap.stanford.edu/data/email-Eu-core.html

## Libraries Used

- `networkx`: For graph construction and analysis
- `matplotlib`: For data visualisation
- `numpy`: For numerical computations
- `gzip`: For reading compressed data files

## Analysis Methods

### 1. Graph Construction
- Created a directed graph using NetworkX
- Nodes represent email users
- Directed edges represent email communications
- Added department labels as node attributes

### 2. Degree Analysis
- Calculated in-degree and out-degree distributions
- Visualised degree distributions using histograms
- Computed average and maximum degrees

### 3. Clustering Analysis
- Calculated average clustering coefficient
- Used undirected graph approximation for clustering analysis

### 4. Centrality Measures
- Computed various centrality measures to identify important nodes
- Analysed node importance based on their position in the network

## Key Findings

1. **Degree Distribution**
   - Average in-degree: 25.44
   - Average out-degree: 25.44
   - Maximum in-degree: 212
   - Maximum out-degree: 334

2. **Clustering**
   - Average clustering coefficient: 0.399

3. **Network Structure**
   - The network shows a typical social network structure
   - Presence of hubs (nodes with high degree)
   - Evidence of community structure based on departments

## Usage

To run the analysis:
1. Ensure all required libraries are installed
2. Place the dataset files in the working directory
3. Run the Jupyter notebook `analysis.ipynb`

## Requirements

- Python 3.x
- NetworkX
- Matplotlib
- NumPy

## License

This project is open source and available under the MIT License. 

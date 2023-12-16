# Social-Network-Analysis-on-Connections

## Overview
This repository contains a Jupyter Notebook (`social_network_zhora_stepanyan.ipynb`) outlining a marketing analytics project for ConnectTel, a hypothetical telecom solutions provider. The notebook includes data analysis, network creation, centrality calculations, and community detection for targeted marketing.

## Table of Contents
- [Introduction](#introduction)
- [Folder Structure](#folder-structure)
- [Usage](#usage)
- [Functions](#functions)
- [Data Sources](#data-sources)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Jupyter Notebook `social_network_zhora_stepanyan.ipynb` details a comprehensive marketing analytics project. It includes code and explanations for various steps involved in the project.

## Folder Structure
- **data:** Contains 'connections.txt', which includes the list of edges used to create the directed graph for network analysis.
- **visualizations:** Stores generated visualizations of graphs, influential nodes, and community structures.

## Usage
To explore the project:
1. Open the Jupyter Notebook (`social_network_zhora_stepanyan.ipynb`) in Jupyter Notebook or JupyterLab.
2. Follow the instructions and code cells in the notebook sequentially to understand the analysis steps and results.

## Functions
### Functions Used in the Code

#### `load_data_from_file(file_path)`
Reads data from a specified file path ('connections.txt') containing edge information and parses it to create a list of edges.

#### `create_directed_graph(edges)`
Constructs a directed graph using NetworkX from the parsed edges obtained earlier.

#### `visualize_graph(graph)`
Visualizes the directed graph using NetworkX and Matplotlib, offering a visual representation of connections.

#### `find_bridges(graph)`
Identifies and returns nodes that are part of bridge edges within the graph, highlighting potential weak points in connections.

#### `calculate_graph_density(graph)`
Calculates the graph density, signifying the level of interconnectedness among nodes and aiding in understanding overall connectivity.

#### `find_highest_lowest_degree_nodes(graph)`
Finds and returns nodes with the highest and lowest degrees in the graph, helping identify highly and less connected nodes.

#### `calculate_centrality_measures(graph)`
Computes centrality measures like closeness, betweenness, and eigenvector centrality for nodes, identifying influential nodes.

#### `detect_communities(graph)`
Applies community detection algorithms to identify distinct communities within the graph, revealing group structures or clusters.

#### `remove_top_nodes_by_centrality(graph, centrality_measure)`
Removes the top three nodes based on specified centrality measures (e.g., degree, closeness, betweenness) and visualizes the updated graph.

#### `identify_top_influencers(graph, communities)`
Identifies and displays top influencers within the top three communities detected in the graph, highlighting influential nodes within communities.


## Data Sources
- **connections.txt:** Contains the list of edges representing connections between nodes in the network.

## Contributing
Contributions to enhance analysis, improve algorithms, or refine visualizations are welcome! Feel free to create issues or pull requests.

## License
This project is licensed under the [MIT License](LICENSE).

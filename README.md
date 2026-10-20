
# AI-Based Road Network Pathfinding System

### Comparing Dijkstra's Algorithm, A*, and Custom Turn-Penalty A*

## Project Overview

## Research Paper PDF here: [Shortest_Path_Search_and_Route_Complexity_Aware_A__on_the_University_of_Minnesota_Walkable_Campus_Network.pdf](https://github.com/user-attachments/files/33737201/Shortest_Path_Search_and_Route_Complexity_Aware_A__on_the_University_of_Minnesota_Walkable_Campus_Network.pdf)



## This project was collaboratively developed by two University of Minnesota students.

Vijay Gururaj – Software development, algorithm implementation, testing, and analysis.

Rahil Sheth – Software development, algorithm implementation, testing, and analysis.

Both contributors participated in the development and evaluation of the pathfinding system

## Technologies Used

- **Python** – Core programming language
- **Google Colab** – Development environment
- **OSMnx** – Retrieval and analysis of real-world pedestrian networks
- **NetworkX** – Graph representation and shortest-path algorithms
- **Pandas** – Data processing and algorithm comparisons
- **Matplotlib** – Route visualization and performance analysis
- **Heapq** – Priority queue implementation for custom A*

## Pathfinding Algorithms

### 1. Dijkstra's Algorithm
Calculates the shortest route between two locations based on weighted path distances.

### 2. A* Search Algorithm
Uses a geographic distance heuristic to guide the search toward the destination.

### 3. Custom Turn-Penalty A*
Extends A* by incorporating additional costs for turns, encouraging routes with reduced navigation complexity.

The custom algorithm applies:
- Left-turn penalty: 50
- Right-turn penalty: 20

These penalties are added to route distance to calculate a complexity-adjusted routing cost.

## Key Features

- Real-world pedestrian network modeling using OpenStreetMap
- Campus landmark identification and graph-node mapping
- Three pathfinding algorithm implementations
- Automated route comparisons between campus landmarks
- Execution-time and route-distance analysis
- Turn-count and route-complexity evaluation
- Campus network and route-density visualizations
- Identification of centrally located campus landmarks

## Performance Evaluation

The project compares algorithms using the following metrics:

| Metric | Description |
|---|---|
| Execution Time | Time required to calculate a route |
| Path Distance | Total walking distance in meters |
| Realistic Cost | Distance plus turn penalties |
| Total Turns | Number of significant direction changes |
| Route Nodes | Number of graph nodes along the route |

The analysis also identifies cases where the custom A* algorithm chooses a different route from Dijkstra's algorithm.

## How to Run

1. Open the project notebook in Google Colab.
2. Install OSMnx using `!pip install osmnx`.
3. Run the notebook cells sequentially.
4. Allow the notebook to retrieve pedestrian network data.
5. Review the algorithm comparison tables and generated visualizations.

An internet connection is required to retrieve OpenStreetMap network data.

## Project Applications

This project demonstrates concepts applicable to:

- GPS navigation and route planning
- Geographic information systems
- Graph search and optimization
- Transportation network analysis
- Algorithm performance benchmarking

## Future Improvements

- Interactive selection of starting points and destinations
- Accessibility-aware routing
- Real-time traffic or pedestrian congestion integration
- Additional heuristic optimization techniques
- Interactive web-based route visualization

## Project Environment

Developed in Python using Google Colab with geographic data from OpenStreetMap.

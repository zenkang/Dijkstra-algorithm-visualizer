# Dijkstra Algorithm Visualizer

A web-based visualization tool for Dijkstra's shortest path algorithm. This interactive application helps users understand how Dijkstra's algorithm works by providing a visual representation of the pathfinding process. This project was created as an educational tool to visualize Dijkstra's algorithm for my algorithms class.

## Live Demo

Visit the live application: [https://zenkang.github.io/Dijkstra-algorithm-visualizer/](https://zenkang.github.io/Dijkstra-algorithm-visualizer/)

## Features

- Interactive graph visualization
- Step-by-step algorithm execution
- Visual representation of shortest path discovery
- Real-time distance calculations and updates
- Node and edge creation interface
- Clear visualization of visited nodes and current frontier
- Shortest path highlighting
- User-friendly interface with intuitive controls
- Responsive design for various screen sizes

## Technologies Used

- HTML5 - Structure and markup
- CSS3 - Styling and layout
- JavaScript - Algorithm implementation and interactivity
- Canvas API - Graph rendering and visualization
- GitHub Pages - Static site hosting

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Git (for development and local setup)
- Basic understanding of graph theory concepts (optional but helpful)

### Installation and Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/zenkang/Dijkstra-algorithm-visualizer.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Dijkstra-algorithm-visualizer
   ```

3. Open `index.html` in your web browser or use a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have http-server installed)
   npx http-server
   
   # Using PHP (if available)
   php -S localhost:8000
   ```

4. Open your browser and navigate to `http://localhost:8000`

## How to Use the Visualizer

1. Open the application in your web browser
2. Create nodes by clicking on the canvas or designated areas
3. Connect nodes by selecting two nodes to create weighted edges
4. Set the source (starting) node and destination (target) node
5. Configure edge weights if the interface allows
6. Run the Dijkstra algorithm visualization
7. Observe the step-by-step process as the algorithm explores nodes
8. View the final shortest path highlighted in the graph

### Understanding the Visualization

- **Unvisited nodes**: Typically shown in one color (e.g., white or light gray)
- **Current node**: The node currently being processed (often highlighted)
- **Visited nodes**: Nodes that have been fully processed (usually darker color)
- **Frontier nodes**: Nodes discovered but not yet processed
- **Shortest path**: The final optimal path from source to destination
- **Distance labels**: Current shortest known distance from source to each node

## About Dijkstra's Algorithm

Dijkstra's algorithm is a fundamental graph search algorithm that solves the single-source shortest path problem for graphs with non-negative edge weights. Developed by computer scientist Edsger W. Dijkstra in 1956, it is widely used in network routing protocols, GPS navigation systems, and many other applications.

### Algorithm Overview

1. **Initialization**: Set the distance to the source node as 0 and all other nodes as infinity
2. **Priority Queue**: Maintain a priority queue of unvisited nodes ordered by their current shortest distance
3. **Relaxation**: For each node, examine its neighbors and update their distances if a shorter path is found
4. **Marking**: Mark the current node as visited once all its neighbors have been examined
5. **Termination**: Continue until all nodes are visited or the destination is reached

### Time Complexity

- **Using a binary heap**: O((V + E) log V) where V is vertices and E is edges
- **Using a Fibonacci heap**: O(E + V log V)
- **Space complexity**: O(V) for storing distances and previous nodes

### Educational Purpose

This visualizer was created specifically for educational purposes in an algorithms class to help students understand:
- How the algorithm systematically explores the graph
- The concept of relaxation and distance updates
- Why the algorithm guarantees finding the shortest path
- The difference between visited and unvisited nodes
- How the priority queue (or similar structure) guides the exploration

## Contributing

Contributions are welcome! This project was created for educational purposes, and improvements that enhance the learning experience are especially appreciated.

### How to Contribute

1. Fork the project
2. Create your feature branch (`git checkout -b feature/educational-enhancement`)
3. Commit your changes (`git commit -m 'Add detailed algorithm explanation'`)
4. Push to the branch (`git push origin feature/educational-enhancement`)
5. Open a Pull Request

### Contribution Ideas

- Add step-by-step algorithm explanation text
- Implement different graph layouts or examples
- Add animation speed controls
- Include algorithm complexity analysis
- Add support for negative edge weights (Bellman-Ford algorithm)
- Implement A* algorithm comparison
- Add more detailed commenting in the code
- Improve accessibility features
- Add mobile touch support

## Technical Implementation

### Project Structure

```
├── index.html          # Main HTML structure
├── styles.css          # CSS styling and layout
├── script.js           # JavaScript algorithm implementation (if separate)
└── README.md           # Project documentation
```

### Key Components

- **Graph Representation**: How nodes and edges are stored and managed
- **Visualization Engine**: Canvas or SVG-based rendering system
- **Algorithm Implementation**: Core Dijkstra's algorithm logic
- **User Interface**: Controls for graph creation and algorithm execution
- **Animation System**: Step-by-step visualization timing and updates

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**zenkang** - [GitHub Profile](https://github.com/zenkang)

*This project was created as an educational tool for an algorithms class to help visualize and understand Dijkstra's shortest path algorithm.*

## Acknowledgments

- Inspired by classic algorithm visualization tools and educational resources
- Created for academic learning and teaching purposes
- Thanks to the algorithms class for providing the motivation to build this visualization tool
- Edsger W. Dijkstra for developing this fundamental algorithm
- The computer science education community for emphasizing the importance of algorithm visualization
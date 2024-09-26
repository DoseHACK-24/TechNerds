# 🚗 Warehouse Autobot Navigation System

Welcome to the **Warehouse Autobot Navigation System**! 🚀 This project aims to guide autobots through a grid, helping them avoid obstacles and, more importantly, each other. Think of it as the ultimate traffic control system for robots! 🤖🚦

## 🧐 Problem Overview

**Dosepacker Inc.** (our imaginary warehouse overlord) has been struggling with autobots getting stuck and crashing into each other. This situation is not only frustrating but also detrimental to business operations. Our goal is to build a robust navigation system that allows these autobots to move safely and efficiently within the warehouse environment.

### Key Challenges

1. **Avoid Collisions**: 
   - No autobot shall collide! 🚫🤖🤖 We need a system that ensures autobots navigate around each other without crashing.
   
2. **Dynamic Movement**: 
   - Autobots must follow simple movement commands such as `Forward()`, `Left()`, `Right()`, and `Wait()`. This allows for flexible navigation in the warehouse grid.
   
3. **Obstacle Navigation**: 
   - The warehouse is filled with walls, boxes, and other obstacles (all marked as `X`). The system must navigate around these obstacles to ensure safe passage.

4. **No Deadlocks**: 
   - Avoid situations where the autobots get stuck like a 4-way stop sign! 🚧 We try to implement a deadlock resolution strategy to ensure continuous movement.

## 🌟 Features

- **Graphical User Interface (GUI)**: 
  - Built using Tkinter, providing a visual representation of the grid, bots, goals, and obstacles.
  
- **A* Pathfinding Algorithm**: 
  - Utilizes the A* algorithm to find the shortest path for each autobot to its goal while avoiding obstacles and other bots.
  
- **Obstacle Management**: 
  - Users can dynamically add or remove obstacles by clicking on the grid.
  
- **Performance Metrics**: 
  - Displays performance metrics such as time taken and commands issued by each bot upon reaching their goals.
  
- **Deadlock Detection**: 
  - Tracks waiting times and detects potential deadlocks.

## 🔧 Installation and Usage

### Prerequisites

- Python 3.x
- Tkinter (comes pre-installed with Python)
- `heapq` for the A* algorithm (also comes pre-installed with Python)

## 💡 How It Works

- The autobots are initialized at specific start positions, and their goals are predetermined.
- When the **"Start"** button is clicked, the system calculates paths for each bot using the **A\*** algorithm.
- Each bot moves according to its calculated path, and the GUI updates in real-time to reflect their movements.
- If a collision is detected, the system will mark the colliding bots as "waiting" and implement a deadlock resolution strategy.
- Performance metrics are displayed at the end of the simulation.

## 🛠️ Technologies Used

- **Python**: The primary programming language used for the project.
- **Tkinter**: For building the graphical user interface.
- **Heapq**: For implementing the priority queue required by the A* algorithm.

## 🤝 Contributing

We welcome contributions! If you'd like to enhance the **Warehouse Autobot Navigation System**, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.


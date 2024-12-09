# 🐜 Ant Colony Optimization (ACO) for Solving the Travelling Salesman Problem (TSP) 🚚 

This repository implements Ant Colony Optimization (ACO) to solve the Travelling Salesman Problem (TSP), a classic optimization problem where the goal is to find the shortest possible route that visits each city once and returns to the origin city. The algorithm simulates the foraging behavior of ants, leveraging pheromone trails to guide the search for the optimal path. 🌍✨

## Key Features 🔑

- **ACO Algorithm Implementation**: Uses Ant Colony Optimization to simulate ants' behavior for finding the shortest path in the TSP. 🐜
- **Visualization**: Graphs showing the best tours found in each iteration and the route of the best solution. 📈
- **Scalability**: Designed to handle a variety of city sets, from small instances to larger datasets. 🌐

## Algorithm Overview 🧠

The ACO algorithm works through the following stages:

1. **Initialization**: The positions of the cities and the initial pheromone levels are set. 🏙️
2. **Tour Construction**: Ants construct tours by probabilistically selecting cities based on pheromone levels and distance heuristics. 🐜➡️🌆
3. **Pheromone Update**: After all ants complete their tours, pheromones are updated. Shorter tours get higher pheromone deposits. 💧
4. **Evaporation**: Pheromones evaporate over time to avoid stagnation and encourage exploration of new paths. ⏳
5. **Iteration**: The algorithm runs for multiple iterations, continually refining the best solution. 🔄

The TSP problem is solved by optimizing the pheromone distribution to guide ants towards shorter tours. 🏆  

## Requirements 🖥️  

To run the code, you'll need Python 3.x and the following libraries:
- `numpy`
- `pandas`
- `matplotlib`

You can install the required dependencies by running:

```bash
pip install -r requirements.txt
```

## How to Use 🚀
Load City Data: Cities can be loaded from a CSV file containing latitude and longitude coordinates.   
For instance, we use a dataset of cities with capital cities selected and randomly sampled for demonstration. 📍  

## Run the Algorithm: 

Adjust the following parameters to control the algorithm's behavior:  

- alpha: Influence of pheromone on the decision-making process (higher values give more importance to pheromones). 🐜
- beta: Influence of the distance heuristic on the decision-making process (higher values give more importance to distance). 📏
-  initial_pheromone: Initial pheromone value. 💧
- evaporation_rate: Rate at which pheromones evaporate each iteration. ⏳
- iterations: Number of iterations the algorithm will run. 🔄

## Visualize Results: 📝

The algorithm outputs two graphs:  
1. Best Tour Path: The best route found by the ants. 🛣️  
2. Tour Length Over Iterations: A graph showing the evolution of the best tour length over time. 📉  

Customize: The code is modular and customizable. You can easily update the cities' data or tweak the algorithm's parameters to suit your needs. ⚙️

## Contributing 🤝
We welcome contributions! If you'd like to improve this project, please feel free to fork the repository, create a branch, and submit a pull request. Whether it's fixing a bug, adding features, or improving the documentation, your help is appreciated. 💡

## License 📜
This project is licensed under the MIT License - see the LICENSE file for details. ⚖️

## Acknowledgments 🙏
This algorithm is inspired by the work of Marco Dorigo on Ant Colony Optimization.   
If you are interested in the theoretical background, refer to the following papers:  
Dorigo, M., & Gambardella, L. M. (1997). "Ant Colony System: A Cooperative Learning Approach to the Traveling Salesman Problem." IEEE Transactions on Evolutionary Computation.
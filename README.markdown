# AI-Based 64-Puzzle Solver with Graph Traversal Visualization 

## Overview

This project implements an AI-based solver for the 64-Puzzle (8x8 sliding tile puzzle), an extension of the classic 15-puzzle, using the A\* search algorithm with the Manhattan Distance heuristic. The solver is integrated with a Tkinter-based GUI for interactive puzzle generation and solution visualization. Additionally, it uses NetworkX and Matplotlib to visualize the state space traversal as a directed graph, providing insights into the AI's search process. The project was developed as part of an Artificial Intelligence course to demonstrate informed search techniques and graph-based visualization.

## Objectives

- Develop an AI agent to optimally solve the 64-Puzzle using the A\* algorithm.
- Implement the Manhattan Distance heuristic for efficient cost estimation.
- Visualize the AI's state space traversal using NetworkX and Matplotlib.
- Create an interactive Tkinter GUI for puzzle simulation and animation.
- Analyze the performance of A\* on large state spaces.

## Features

- Randomized puzzle generation with user-defined scramble steps.
- A\* algorithm with Manhattan Distance heuristic for optimal pathfinding.
- Interactive GUI displaying puzzle states and move animations.
- Graph visualization of the search space showing state transitions.
- Support for an 8x8 grid with 64 tiles, including a blank tile.

## Project Report Summary

The project report details the development and evaluation of the 64-Puzzle solver:

- **Methodology**: Utilizes A\* with Manhattan Distance heuristic, ensuring admissible and consistent cost estimation. A directed graph tracks state transitions.
- **Game Mechanics**: The 8x8 grid allows tiles to slide into the blank space, aiming for an ordered arrangement (1 to 63, blank at the end).
- **Implementation**: Built with Python, Tkinter for GUI, NetworkX for graph construction, and Matplotlib for visualization.
- **Evaluation**: Effective for lower scramble depths (10–20 steps), but computationally intensive for higher depths (50+ steps) due to the large state space (64! permutations).
- **Challenges**: Managing memory usage and ensuring GUI responsiveness for complex puzzles.
- **Future Work**: Implementing IDA\* for memory efficiency, adding pattern databases, and supporting manual user moves.

For full details, refer to the project report (`report.pdf`) in the repository.

## Requirements

- Python 3.8 or higher
- Libraries:
  - `networkx` (for graph construction)
  - `matplotlib` (for graph visualization)
  - Standard libraries: `tkinter`, `heapq`, `random`, `time`

## Evaluation & Results

- Tested with scramble steps ranging from 10 to 50.
- Performs well for 10–20 steps with acceptable real-time performance.
- Higher scramble depths (50+) increase memory and computation demands, highlighting A\*'s limitations in large state spaces.
- Graph visualization effectively illustrates node expansion and path selection.

## Authors

- Muneeb Baig (22K-5095)
- Rafay Ahmed (22K-5030)

## Acknowledgments

- Instructor: Ms. Almas Ayesha Ansari
- Course: Artificial Intelligence

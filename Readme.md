# N-Queen Problem Solver

This project implements two different approaches to solve the N-Queen problem :
1. Genetic Algorithm
2. Stochastic Hill Climbing

## Problem Description

The N-Queen problem is a classic chess puzzle where the challenge is to place N queens on an N×N chessboard so that no two queens threaten each other. This means that no two queens should share the same row, column, or diagonal.

## Implementations

### 1. Genetic Algorithm (GA) Implementation

The GA implementation (`N-Queen-GA.ipynb`) uses the following components:

- **Fitness Function**: Calculates the number of conflicts between queens
- **Selection**: Tournament selection with k=3 participants
- **Crossover**: Two-point crossover
- **Mutation**: Random swap mutation with 5% probability
- **Parameters**:
  - Population Size: 100
  - Number of Generations: 500
  - Mutation Rate: 0.05
  - Board Size: 32×32

### 2. Stochastic Hill Climbing Implementation

The Hill Climbing implementation (`N-Queen.ipynb`) uses:

- **Heuristic Function**: Measures the number of conflicts between queens
- **Neighbor Generation**: Random swap of queen positions
- **Parameters**:
  - Board Size: 8×8
  - Maximum Iterations: 5000
  - Number of Restarts: 20
  - Number of Neighbors (k): 4

## Solution Encoding

The solutions are encoded as permutations where:
- The index represents the column number (0-based)
- The value represents the row number (1-based)

For example, `[2,1,3,4]` represents:
```
0 ♕ 0 0
♕ 0 0 0
0 0 ♕ 0
0 0 0 ♕
```

## Author

**Yasin Pourraisi**
- GitHub: [yasinpurraisi](https://github.com/yasinpurraisi)
- Email: yasinpourraisi@gmail.com
- Telegram: [yasinprsy](https://t.me/yasinprsy)

## Requirements

- Python 3.x
- Jupyter Notebook

# River Crossing with A* Search Algorithm

This project solves the classic River Crossing Problem using the A* search algorithm.  
It was developed as part of the Artificial Intelligence course at the Athens University of Economics and Business.

## Problem Description
A family must cross a river at night using a log that can carry only two people at a time.  
They must carry a torch, and each person has a different crossing time.  
When two people cross, the slower one dictates the time.  

Goal: Find the optimal sequence of moves (pairings and directions) that minimizes the total crossing time.  

## Technologies
- Language: Java
- Algorithm: A\* (A-star) search
- Heuristic: maximum remaining crossing time

## File Structure
src/
Main.java         # entry point
AstarSearch.java  # A* algorithm implementation
State.java        # models the problem state

## How to Build & Run

### Compile
javac src/*.java

## Run
java -cp src Main

## Sample Input
Enter the number of people: 5
Enter the total time (in minutes): 30
Enter the time required for each person to cross the river:
1 3 6 8 12

## Sample Output
The family crosses in optimal total time = 30 minutes
For 6 persons with times [1, 3, 6, 8, 12, 15], total = 40 minutes.

## What I Learned
- Implementing A* search with admissible heuristics
- Representing problems as state spaces in AI
- Designing custom heuristics for performance
- Applying AI algorithms to classic puzzle problems
- Writing clean, modular Java code

## Continuous Integration

- This repo includes a GitHub Actions workflow (ci-java.yml) that:
  - Compiles all Java source files
  - Runs the Main class with a small test input


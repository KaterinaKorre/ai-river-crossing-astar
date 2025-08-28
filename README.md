# River Crossing with A* Search Algorithm

This project solves the classic River Crossing Problem using the A* search algorithm. It was developed as part of the "Artificial Intelligence" course at AUEB.

## Course Details

- Course: Artificial Intelligence
- Semester: Ε (Spring 2023–24)

## Problem Description

A family must cross a river at night using a log that can carry only two people at a time. They must carry a single torch, and each person has a different crossing time. When two people cross, the slower one dictates the time.

The goal is to find the optimal sequence of moves (pairings and directions) that minimizes the total crossing time.

See `assignment_description.pdf` for full problem description and constraints.

## Technologies

- Language: Java
- Algorithm: A* (A-star) Search
- Heuristic: Maximum remaining crossing time

## File Structure

- `src/`: Source code folder
  - `Main.java`: Entry point
  - `AstarSearch.java`: Contains A* algorithm implementation
  - `State.java`: Models a river crossing state
- `Report.pdf`: Explanation of algorithm design and experimental results
- `assignment_description.pdf`: Official problem statement from instructor

## Results

- N = 5 persons: Total crossing time = 30
- N = 6 persons: Total crossing time = 40

(see `Report.pdf` for full terminal outputs and explanation)

## Run Instructions

1. Compile all source files: javac src/*.java

2. Run the main class: java -cp src Main

## Sample Input

Enter the number of people: 5
Enter the total time (in minutes): 30
Enter the time required for each person to cross the river:
1 3 6 8 12

## Notes

- The program stops if no solution exists within the given maximum total time.
- The heuristic is admissible, calculated as the max crossing time of remaining people on the starting side.




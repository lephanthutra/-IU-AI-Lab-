# -IU-AI-Lab-
This is my solutions from lab session of "Introduction to Artificial Intelligence" course.

# Lab 00
This lab has 5 problems to let you get familiar with Python.

# Lab 1

## Depth First Search

1. **Idea**:  The algorithm starts at the root node or arbitrary node and explores as far as possible along each branch before backtracking. The basic idea is to start from the root or any arbitrary node and mark the node, then move to the **adjacent unmarked node** and continue this loop until there is **no unmarked adjacent node**. Then backtrack and check for other unmarked nodes and traverse them. Finally, print out the nodes in the path.

2. **Algorithm**: 

- Create a recursive function that takes the index of the node and a visited array.

- Mark the current node as visited and print the node.

- Traverse all the adjacent and unmarked nodes and call the recursive function with the index of the adjacent node.

- Run a loop from 0 to the number of vertices and check if the node is unvisited in the previous DFS, call the recursive function with the current node.

## Breadth First Search

1. **Idea**: 

2. **Algorithm**:

## Uniform Cost Search

## A Star Search



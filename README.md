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

- Traverse all the adjacent unmarked nodes and call the recursive function with the index of the adjacent node.

- Run a loop from 0 to the number of vertices and check if the node is unvisited in the previous DFS, call the recursive function with the current node.

## Breadth First Search

1. **Idea**: Constrast to DFS, the basic idea of BFS is to start find a path from the root node at depth level to the node at next depth level as short as possible.

2. **Algorithm**:

The algorithm uses a queue data structure to store vertices that will be traversed in order of width priority.

**Step 1: Initialize***

- The vertices are in the unsigned state. Except the source vertex ***s*** has been marked.

-  An initial queue contains only one element, ***s***.

**Step 2: Repeat the following steps until the queue is empty:**

- Remove vertex ***u*** from the queue.

- Consider all unmarked vertices ***v*** adjacent to ***u***, for each of those vertices ***v***:
   
   * Mark ***v*** visited.
   
   * Record the path from ***u*** to ***v***.
   
   * Push ***v*** into the queue (vertex ***v*** will wait for approval in the following steps).
   
**Step 3: Tracing to find the way.**

## Uniform Cost Search

1. **Idea**: The basic idea of UCS is to use the lowest cumulative cost to find a path from the source to the destination.

2. **Algorithm**:

- Insert the root node into the priority queue

- Repeat while the queue is not empty:
  
  * Remove the element with the highest priority
    
    ***If*** the removed node is the destination, print total cost and stop the algorithm

    ***Else***, enqueue all the children of the current node to the priority queue, with their cumulative cost from the root as priority


## A Star Search



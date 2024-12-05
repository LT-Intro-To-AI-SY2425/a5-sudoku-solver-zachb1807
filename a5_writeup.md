# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

The efficiency of the depth first search tends to be better at solving the sudoku puzzles because it can go in depth to search for possible solutions, rather than waiting for all the broad searches to be completed before moving down a level.



2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

The primary difference between implementing the two data structures was that DFS required pulling from the most recently added items from the stack, while BFS required pulling from the oldest items in the queue to test for potential solutions. I can't think of any other data structures or algorithms that could have been used to solve this.



3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
You can implement the same idea of brute-force testing all the possible combinations to other puzzles such as chess or crosswords. The lessons about trial and error as well as the difference between a Stack and a Queue can be applied to real-world problems like pathfinding or scheduling. It also exposes the flaws in this method of problem-solving, as it can be very slow and inefficient for larger puzzles or problems.
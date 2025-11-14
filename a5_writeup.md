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

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them? Basically some things I learned is how a BFS and DFS algrothim work and the differences between them and the purposes of using them like queue and stack with how it back tracks and whichever one is better for the situation, a challenge that can be seen in my code is the assert means something in my code for the DFS and BFS is wrong. How I fixed it is i didnt pus the board to the BFS or DFS so they couldn't solve it but then when i added it, it fixed.



2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems? A program I could apply this to in a future project or program is possibly a crossword program. But a real world scenairo where DFS or BFS might be useful is for a GPS system where it gvies the possiblities of what time you could arrive at your destination and make decision is an accident happens recent or what not. Another constraint satifsfaction problems is a battleship program. 



3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?
Basically how a stack and queue class works, is a stack is a LIFO where the last item put inside is the the first one that leaves, while a queue is a FIFO where the first item that gets put in is the first one to leave. They are important for BFS and DFS algorithms, is a DFS goes through all the items in branch then it starts backtracking so you would use a stack so it could go through the entire path and then backtracks to the other path. While BFS which is good for queue because it searchs through its current level and then goes to the next level when its current level is correct and it always goes through all the levels. Queue is the best for BFS because it searchs through all the levels but before it goes to the next level it checks its current level making sure its right. While Stack is the best for DFS because it searches the deepest that hasn't yet been tested and tests it all the way through until it hits a dead end.
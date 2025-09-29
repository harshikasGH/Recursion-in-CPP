Recursion in C++

Aim  
To study and understand the concept of **recursion in C++**, and explore how problems can be solved by functions calling themselves until a base condition is reached.

Theory  
**Recursion** is a programming technique in which a function calls itself directly or indirectly to solve a problem.  
The problem is broken into **smaller subproblems of the same type**, and the process continues until a **base case** is satisfied.  

Key Points  
- **Recursive Function:** A function that calls itself.  
- **Base Case:** The terminating condition that stops recursion.  
- **Recursive Case:** The part of the function where it calls itself with a smaller/simpler input.  
- **Call Stack:** Each recursive call is stored in memory; when the base case is reached, the stack unwinds and results are returned.  

Types of Recursion  
1. **Direct Recursion** – Function calls itself directly.  
2. **Indirect Recursion** – Function A calls B, and B calls A.  
3. **Tail Recursion** – Recursive call is the last operation.  
4. **Non‑Tail Recursion** – Recursive call is followed by extra work.  
5. **Linear Recursion** – Only one recursive call per step.  
6. **Tree Recursion** – Multiple recursive calls per step.  

Algorithms  
Factorial using Recursion  
1. **Start**  
2. Input an integer `n`.  
3. Define recursive function `fact(n)`:
   - If `n == 0`, return `1` (**base case**).  
   - Else, return `n * fact(n-1)` (**recursive case**).  
4. Call `fact(n)` from `main()`.  
5. Display the result.  
6. **End**

Sum of Natural Numbers using Recursion  
1. **Start**  
2. Input an integer `n`.  
3. Define recursive function `sum(n)`:
   - If `n <= 1`, return `n` (**base case**).  
   - Else, return `n + sum(n-1)` (**recursive case**).  
4. Call `sum(n)` from `main()`.  
5. Display the result.  
6. **End**

 String Reversal using Recursion  
1. **Start**  
2. Input a string `str`.  
3. Find the length of the string `n`.  
4. Define recursive function `reverse(str, i, n)`:
   - If `i == n`, stop (**base case**).  
   - Else, call `reverse(str, i+1, n)` (**recursive case**).  
   - After returning, print `str[i]`.  
5. Call `reverse(str, 0, n)` from `main()`.  
6. Display the reversed string.  
7. **End**

Applications of Recursion  
Recursion is widely used in **mathematics, algorithms, and data structures**. Some key applications include:

- **Mathematical Computations**  
  - Factorial, Fibonacci series, power functions, GCD.  

- **Searching and Sorting**  
  - Binary Search, Merge Sort, Quick Sort.  

- **Data Structures**  
  - Traversal of trees (preorder, inorder, postorder).  
  - Graph traversal (DFS).  
  - Linked list operations.  

- **Backtracking Problems**  
  - N‑Queens problem.  
  - Sudoku solver.  
  - Maze pathfinding.  

- **String and Array Operations**  
  - Reversing strings.  
  - Palindrome checking.  
  - Generating permutations and combinations.  

Conclusion  
This study of recursion in C++ demonstrates:  

- **Self‑Referential Nature** – Functions can call themselves to solve problems.  
- **Base Case Importance** – Prevents infinite recursion and stack overflow.  
- **Code Simplification** – Complex problems become easier to express.  
- **Applications** – Factorial, sum of numbers, string reversal, sorting, searching, and tree/graph traversal.  

Recursion is elegant and powerful, but must be used carefully due to memory and performance considerations.

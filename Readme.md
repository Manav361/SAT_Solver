# Sudoku pair: solving and generation
* I have to write a k-sudoku puzzle pair solver and generator by encoding the problem to propositional logic and solving it via a SAT solver (https://pysathq.github.io/). 

Given a sudoku puzzle pair S1, S2 (both of dimension k) as input, my job is to write a program to fill the empty cells of both sudokus such that it satisfies the following constraints
* Individual sudoku properties should hold.
* For each empty cell S1[i, j] ≠ S2[i, j], where i is row and j is column.

#### Input: 
Parameter k, single CSV file containing two sudokus. The first k * k rows are for the first sudoku and the rest are for the second sudoku. Each row has k * k cells. Each cell contains a number from 1 to k * k. Cell with 0 specifies an empty cell.
Output: If the sudoku puzzle pair doesn't have any solution, you should return None otherwise return the filled sudoku pair.

In the second part, I have to write a k-sudoku puzzle pair generator. The puzzle pair must be maximal (have the largest number of holes possible) and must have a unique solution. 
* Input: Parameter k
* Output: CSV file containing two sudokus in the format mentioned in Q1.


# Largest-Local-Values-in-Matrix
LeetCode problem 2373
# Intuition
In Dynamic Programming, we break problem into subproblems and then we solve subproblems one by one to get result. In this question I hav edone the same.

# Approach
We create two array(table, ans). table stores intermediate solution of subproblem. ans stores final answer and the we return it.

1st Loop --> In this loop we use table which has 2 rows less than original array grid. In this we pick first 3 values of each columns and we find the largest and store it in table array. In this way we get all the largest value of all columns of 3X3 matrix and store it in table array.

2nd Loop --> In this loop we compare each columns largest value which we have stored in table array. And then we store that value in ans array. We return this array. 

DP -> we divided problem which was to get largest of each 3X3 matrix into smaller subproblems. For each 3X3 matrix we first calculate maximum of each column. Then we get a result of 1X3 matrix for each 3X3 matrix. Then we compare each of these to get final answer.

# Complexity
- Time complexity:
O(n^2) --> We are using two loops to iterate through all the subproblems

- Space complexity:
O(n^2) --> We are defining two arrays for storing solution of intermediate subproblems. 

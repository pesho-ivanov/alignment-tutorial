# Dynamic programming (DP)

> DP is a powerful technique for combinatorial problems, such as optimization
> and counting. A problem is recursively split into overlapping subproblems,
> such that the solutions of the subproblems can be merged into to a solution of
> the bigger problem. Introduced by [Bellman
> (1954)](https://www.semanticscholar.org/paper/On-the-Theory-of-Dynamic-Programming.-Bellman/dc9047917d1ceb3805d954c73899ddd2d40dd5eb)

DP [@bellman1954theory]
\bibliography

TODO: picture of exponentially many overlapping alignment subproblems

Distinguish from **Divide&Conquere**:

* DP is about skipping recomputation for the same subtask. This could lead to an exponential acceleration.
* The subtasks for D&C are independent: they don't overlap so cannot be reused.

Distinguish from **Greedy** (assuming an optimization task):

* DP considers all possible steps that lead to a subtask solution -- at least one of them must bring an optimal solution
* Note that some greedies can also be provably optimal/correct.

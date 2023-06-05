This is where the Diffing Algorithm comes into play. Some concepts used by this Algorithm are:

1 Two elements of different types will produce different trees.

2. Breadth-First Search (BFS) is applied because if a node is found as changed, it will re-render the entire subtree hence Depth First Approach is not exactly optimal.

3. When comparing two elements of the same type, keep the underlying node as same and only update changes in attributes or styles.

4. React uses optimizations so that a minimal difference can be calculated in O(N) efficiently using this Algorithm.
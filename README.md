# Python implements the Min-Heap algorithm

A Min-Heap is a complete binary tree where the value in each internal node is less than or equal to the value in the children of that node.

A min heap is a specialized tree-based data structure that satisfies the heap property. In a min heap, for any given node I, the value of I is less than or equal to the values of its child nodes. This ensures that the smallest element is at the root of the heap.
Mapping the elements of a heap into an array is trivial: if a node is stored at index # k  , its left child is stored at index   # 2k+1  and the right child is stored at index # 2k+2  for 0-based indexing , and for 1  - based  indexing , the left child is at  2k and the right child is at  # 2k+1 .

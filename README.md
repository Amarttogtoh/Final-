# Python implements the Min-Heap algorithm

A Min-Heap is a complete binary tree where the value in each internal node is less than or equal to the value in the children of that node .

A min heap is a specialized tree-based data structure that satisfies the heap property. In a min heap, for any given node I, the value of I is less than or equal to the values of its child nodes. This ensures that the smallest element is at the root of the heap.
Mapping the elements of a heap into an array is trivial: if a node is stored at index **k** , its **left child** is stored at index   **2k+1**  and the right **child** is stored at index **2k+2**  for **0-based indexing** , **and for 1** - based  **indexing** , the left child is at  **2k** and the right child is at  **2k+1**.

# Min-heap example: 
![image](https://github.com/user-attachments/assets/627f253b-477c-4184-9353-ec5ca1da4810)

# How is a Min Heap represented?

A Min Heap is a complete binary tree. A Min Heap is usually represented as an array. The root element will be at  **Arr[0]**. For any i nodes,  **Arr[i]** :
•	**Arr[(i -1) / 2]**  returns its parent node.

•	**Arr[(2 * i) + 1]**  returns its left child.

•	**Arr[(2 * i) + 2]**  returns its right child.

# Operations on the minimum heap:
1.	**getMin()** : Returns the root element of the Min Heap. The time complexity of this operation is **O(1)**.
2.	**extractMin()** : Removes the minimum element from MinHeap. The time complexity of this operation is  **O(Log n)** because this operation requires maintaining the heap properties (by calling heapify()) after removing the root.
3.	**insert()** : Inserting a new key takes  **O(Log n)**  time. We add a new key at the end of the tree. If the new key is greater than its parent key, we don't need to do anything. Otherwise, we need to traverse to fix the violated heap property.

   Following is the implementation of Min Heap in Python –
   
![image](https://github.com/user-attachments/assets/c5ab0133-4ce5-488d-b280-1e30b13dbcb2)


   
# Output:

![image](https://github.com/user-attachments/assets/c4a3a281-0141-43b5-919f-80972de0e76c)

# Using Library functions:
We use  the heapq  class to implement Heaps in Python. By default, a min heap is implemented by this class.

![image](https://github.com/user-attachments/assets/cbc6dde3-9883-4b72-97f1-4c615d8bf49c)

# Output: 

![image](https://github.com/user-attachments/assets/a3ad196a-a125-4263-ba35-ae16e1a660fb)

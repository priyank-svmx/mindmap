# 2.5.3 Heap

## Heap Overview
- A specialized binary tree-based data structure.
- Designed to maintain a specific order property, where parent nodes are either greater than (max-heap) or less than (min-heap) their children.

## Properties of a Heap
- **Complete Binary Tree**:
  - Every level, except possibly the last, is completely filled.
  - Nodes are added from left to right.
- **Heap Order Property**:
  - **Min-Heap**: Parent nodes are less than or equal to their children.
  - **Max-Heap**: Parent nodes are greater than or equal to their children.

## Types of Heaps
- **Min-Heap**
  - Root node contains the smallest element.
  - Efficient for retrieving minimum values quickly.
- **Max-Heap**
  - Root node contains the largest element.
  - Efficient for retrieving maximum values quickly.
  
## Core Operations
- **Insert**:
  - Add element to the end of the heap and "bubble up" to maintain heap property.
  - Time Complexity: \(O(\log n)\).
- **Pop (Remove)**:
  - Remove the root element (highest priority).
  - Replace root with the last element and "push down" to maintain order.
  - Time Complexity: \(O(\log n)\).
- **Peek (Top)**:
  - Retrieve the root element without removing it.
  - Time Complexity: \(O(1)\).

## Applications of Heaps
- **Priority Queues**:
  - Commonly implemented using heaps to provide efficient insertion and priority-based removal.
- **Graph Algorithms**:
  - Used in shortest-path algorithms like Dijkstra’s and Prim’s.
- **Sorting**:
  - Basis for Heapsort, which has a time complexity of \(O(n \log n)\) and sorts in-place.

## Advantages of Heaps
- **Efficient Insert and Pop Operations**:
  - Balanced time complexity for inserting and retrieving highest-priority elements.
- **Memory Efficiency**:
  - Can be implemented using arrays, requiring minimal additional memory for tree pointers.

## Limitations of Heaps
- **Inefficient for Ordered Retrieval**:
  - Heaps do not maintain sorted order across all elements, only the root (top priority).
- **Dynamic Priority Adjustments**:
  - Not optimal for frequent priority updates; structures like Fibonacci heaps may perform better in these cases.

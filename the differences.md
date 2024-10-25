# 2.5.4 Priority, Min-Heap, and Max-Heap

## Priority Concept
- **Definition**: A value assigned to elements to determine their order in a queue.
- **Purpose**: Ensures that elements with higher priority are accessed before others.
- **Applications**: Task scheduling, resource allocation, real-time systems.

---

## Min-Heap
- **Structure**: A binary heap where the smallest element is always at the root.
- **Heap Property**: Each parent node is smaller than or equal to its children.
- **Core Operations**:
  - **Insert**: Add element at the end and bubble up to maintain heap property.
    - **Time Complexity**: \(O(\log n)\)
  - **Pop (Remove)**: Remove the root (smallest) element and push down to restore order.
    - **Time Complexity**: \(O(\log n)\)
  - **Peek (Top)**: Retrieve the smallest element without removing it.
    - **Time Complexity**: \(O(1)\)
- **Use Cases**: 
  - Efficiently retrieving minimum values.
  - Applications needing constant access to the smallest element, like shortest path algorithms.

---

## Max-Heap
- **Structure**: A binary heap where the largest element is always at the root.
- **Heap Property**: Each parent node is larger than or equal to its children.
- **Core Operations**:
  - **Insert**: Add element at the end and bubble up to maintain heap property.
    - **Time Complexity**: \(O(\log n)\)
  - **Pop (Remove)**: Remove the root (largest) element and push down to restore order.
    - **Time Complexity**: \(O(\log n)\)
  - **Peek (Top)**: Retrieve the largest element without removing it.
    - **Time Complexity**: \(O(1)\)
- **Use Cases**: 
  - Applications requiring quick access to the largest element, such as in simulations, gaming, and stock price tracking.

---

## Choosing Between Min-Heap and Max-Heap
- **Depends on Priority Definition**: 
  - Use **Min-Heap** if lower values have higher priority (e.g., shortest path).
  - Use **Max-Heap** if higher values have higher priority (e.g., finding largest values quickly).
- **Application-Driven Choice**:
  - **Min-Heap** for minimum retrieval, **Max-Heap** for maximum retrieval.
  - In some applications, both types may be used together to manage different priority types.

---

## Advantages of Min-Heap and Max-Heap
- **Efficient Priority Access**: Both offer \(O(1)\) access to highest-priority element.
- **Balanced Insert and Pop Performance**: \(O(\log n)\) for both operations, ensuring scalability.

## Limitations
- **Non-Ordered Access**: Heaps only guarantee priority at the root; they don’t maintain sorted order across all elements.
- **Dynamic Priority Adjustments**: Updating priorities of existing elements can be costly and complex.

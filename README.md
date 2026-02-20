Count Total Nodes in a Binary Tree (Level Order) – C

This project demonstrates how to count the total number of nodes in a Binary Tree using Level Order Traversal (Breadth-First Search) in C programming language.

The program uses a queue (implemented using an array) to traverse the tree level by level and count nodes.

📌 Description

In this program:

A binary tree is created using dynamic memory allocation.

Level Order Traversal (BFS) is used.

A queue (array-based) is used to visit nodes.

Each visited node increments the counter.

The total number of nodes is displayed.

🧠 Algorithm Used (Level Order Traversal)

Steps:

If the root is NULL, return 0.

Create a queue.

Insert the root into the queue.

While the queue is not empty:

Remove a node from the queue.

Increment count.

Insert left child (if exists).

Insert right child (if exists).

Return the total count.

📂 Data Structure Used
struct Node {
    int data;
    struct Node *left, *right;
};

Each node contains:

data → Value stored in node

left → Pointer to left child

right → Pointer to right child

🌳 Tree Created in Program
        1
       / \
      2   3
     / \
    4   5

Total nodes in this tree = 5

▶️ Sample Output
Total Nodes = 5
⚙️ How to Compile and Run
1️⃣ Compile
gcc count_binary_tree_nodes.c -o count_binary_tree_nodes
2️⃣ Run
./count_binary_tree_nodes
⏱️ Time & Space Complexity

Time Complexity: O(n)
(Each node is visited once)

Space Complexity: O(n)
(Queue storage in worst case)

Where:

n = Number of nodes in the tree

📚 Concepts Covered

Binary Tree

Level Order Traversal

Breadth-First Search (BFS)

Queue Implementation

Tree Node Counting

⚠️ Limitations

Queue size is fixed (50).

No memory deallocation (free() not used).

Tree is manually created.

👨‍💻 Author

Ritik Chauhan

If you want, I can also provide:

Recursive version of node counting

Height calculation version

Full Binary Tree operations (Insert, Delete, Traversals)

Menu-driven tree program

# Day16-50-days-coding-challenge
## 🔹 Problem 1: Delete Node in a Linked List

**Problem Statement:**  
You are given a node in a singly-linked list — **not the head**, and not the **last node**.  
Your task is to delete that node.

- You cannot access the node before it.
- All node values are unique.
- After deletion, the list should remain in the correct order.

### ✅ Example:
- Input: `head = [4,5,1,9], node = 5` → Output: `[4,1,9]`
- Input: `head = [4,5,1,9], node = 1` → Output: `[4,5,9]`

### 💡 Approach:
- Copy the value of the next node into the current node.
- Bypass the next node by updating the current node’s `.next`.

---

## 🔹 Problem 2: Sum of Square Numbers

**Problem Statement:**  
Given a non-negative integer `c`, determine whether there are two integers `a` and `b` such that:  
`a² + b² = c`

### ✅ Example:
- Input: `c = 5` → Output: `true` (1² + 2²)
- Input: `c = 3` → Output: `false`

### 💡 Approach:
- Iterate from `a = 0` to `sqrt(c)` and check if `c - a²` is a perfect square.
- Alternatively, use a **two-pointer** approach starting from `0` and `sqrt(c)`

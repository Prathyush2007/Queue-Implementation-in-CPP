# Queue Implementation  

**Name:** Prathyush
**PRN:** 24070123064 
**Batch:** ENTC A3  

---

## 📌 Overview  

A **Queue** is a linear data structure where insertion takes place at the **rear** and deletion occurs at the **front**.  
It is widely used in **task scheduling, buffering, and resource management**.  

In C++, a queue can be built using arrays, pointers, or the STL `queue` class.  
Here, it is implemented using a **static array** with fixed size.  

### 🔹 Key Operations  
- **Enqueue (Insert):** Add an element at the rear.  
- **Dequeue (Delete):** Remove an element from the front.  
- **Display:** Print all elements from front to rear.  
- **Overflow:** Queue is full, no more insertions allowed.  
- **Underflow:** Queue is empty, no deletions possible.  

---

## 1️⃣ Program: Add, Delete Members in Queue & Check Overflow/Empty  

### 🔹 Algorithm  
1. Initialize queue with `front = -1` and `rear = -1`.  
2. **Enqueue Operation:**  
   - If `rear == SIZE-1`, print **Queue Overflow**.  
   - If `front == -1`, set `front = 0`.  
   - Increment `rear` and insert the new element.  
3. **Dequeue Operation:**  
   - If `front == -1` or `front > rear`, print **Queue Underflow**.  
   - Otherwise, remove element at `front` and increment `front`.  
4. **Display Operation:**  
   - If empty, print **Queue is empty**.  
   - Else, print all elements from `front` to `rear`.  
5. Repeat steps for further operations.  

### 🔹 Theory  
This program implements a **static queue** using arrays:  
- **Insertion (Enqueue):** Adds data sequentially at the rear.  
- **Deletion (Dequeue):** Removes data from the front.  
- **Overflow check:** Prevents adding elements beyond capacity.  
- **Underflow check:** Prevents removing elements when empty.  

Thus, the program demonstrates the working of a **basic static queue**.  

---

## ✅ Sample Output  

10 Inserted into queue.
20 Inserted into queue.
30 Inserted into queue.

Queue elements: 10 20 30

10 Removed from queue.

Queue elements: 20 30

40 Inserted into queue.

Queue elements: 20 30 40

50 Inserted into queue.

Queue Overflow!
Queue Overflow!

Queue elements: 20 30 40 50

yaml
Copy code

---

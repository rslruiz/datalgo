<!--- al06Stacks
--->
## Stacks
A stack is a collection of objects that are inserted and removed according to the
last-in, first-out (LIFO) principle.

### The Stack ADT
A stack is an abstract
data type (ADT) such that an instance S supports the following two methods:

| Method | Description |
| ---: | :--- |
| **S.push(e)**: | Add element e to the top of stack S. |
| **S.pop(&nbsp;)**:| Remove and return the top element from the stack S; an error occurs if the stack is empty.|

Additionally, let us define the following accessor methods for convenience:

| Method | Description |
| ---: | :--- |
|**S.top(&nbsp;)**:| Return a reference to the top element of stack S, without removing it; an error occurs if the stack is empty.|
| **S.is_empty(&nbsp;)**: | Return True if stack S does not contain any elements.|
|**len(S)**:| Return the number of elements in stack S; in Python, we implement this with the special method `__len__` .|

Realization of a stack **S** as an adaptation of a Python list **L**.

| Stack Method | Realization with Python list |
| :--- | :---|
| S.push(e) | L.append(e)|
| S.pop(&nbsp;) | L.pop(&nbsp;) |
| S.top(&nbsp;) | L[−1] |
| S.is empty(&nbsp;) | len(L) == 0 |
| len(S) | len(L) |

## Queues
A stack is a collection of objects that are inserted and removed according to the
first-in, first-out (FIFO) principle.

### The Queue ADT
The ***queue*** abstract data type (ADT)
supports the following two fundamental methods for a queue **Q**:

| Method | Description |
| ---: | :--- |
| **Q.enqueue(e)**: | Add element `e` to the back of queue `Q`. |
| **Q.dequeue(&nbsp;)**: | Remove and return the first element from queue `Q`; an error occurs if the queue is empty. |

The queue ADT also includes the following supporting methods (with first being
analogous to the stack’s top method):

| Method | Description |
| ---: | :--- |
| **Q.first(&nbsp;)**: | Return a reference to the element at the front of queue `Q`, without removing it; an error occurs if the queue is empty. |
| **Q.is_empty(&nbsp;)**: | Return True if queue `Q` does not contain any elements. |
| **len(Q)**: | Return the number of elements in queue `Q`; in Python, we implement this with the special method `__len__` . |

## Double-Ended Queues
A *double-ended queue*, or *deque*, which is usually pronounced “deck” supports insertion and deletion at both the front and the back of the queue.

### The Deque ADT
The ***deque*** abstract data type (ADT)
supports the following methods for a deque **D**:

| Method | Description |
| ---: | :--- |
| **D.add_first(e)**: | Add element e to the front of deque `D`. |
| **D.add_last(e)**: | Add element e to the back of deque `D`. |
| **D.delete_first(&nbsp;)**: | Remove and return the first element from deque D; an error occurs if the deque is empty. |
| **D.delete_last(&nbsp;)**: | Remove and return the last element from deque `D`; an error occurs if the deque is empty.|

Additionally, the deque ADT will include the following accessors:

| Method | Description |
| ---: | :--- |
| **D.first(&nbsp;)**: | Return (but do not remove) the first element of deque `D`; an error occurs if the deque is empty. |
| **D.last(&nbsp;)**: | Return (but do not remove) the last element of deque `D`; an error occurs if the deque is empty. |
| **D.is_empty(&nbsp;)**: | Return True if deque `D` does not contain any elements. |
| **len(D)**: | Return the number of elements in deque `D`; in Python, we implement this with the special method `__len__` .

Ref.: Goodrich, Michael, Roberto Tamassia, and Michael Goldwasser, *Data Structures and Algorithms in Python*, Hoboken, NJ: Wiley, 2013. pp. 228-254

RSLRuiz 2020

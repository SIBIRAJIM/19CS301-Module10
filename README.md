# 19CS301-Module10
### EX: 10.a  STACK
### Aim: 
To Write a python program to get the integer values from the user and push only the odd number into the stack and later pop the last 2 elements.

### Algorithm:

1. Start
2. Input n
3. Initialize an empty list l
4. Repeat n times:
   a. Input m
   b. If m is odd (i.e., m % 2 != 0), append m to list l
5. Print list l (containing only odd numbers)
6. Repeat 2 times:
   a. Remove the last element from l using pop()
7. Print the updated list l
8. End


### Program:
```python
# Name: Nidhish B
# Reg.No: 212223050032

n=int(input())
l=[]
for i in range(n):
    m=int(input())
    if m%2!=0:
        l.append(m)
        
print(l)

for i in range(2):
    l.pop()

print(l)
```

### Output:

![image](https://github.com/user-attachments/assets/57fdc76c-c070-42b0-b23a-6de0038f3ee7)

### Result: 

Thus, the given program is implemented and executed successfully.
 


### EX: 10.2 IMPLEMENTATION OF STACK

### Aim:

To Write a python program to implement the stack using deque method for rotating the stack.

### Algorithm:

1. Start
2. Input n (number of rotation steps)
3. Initialize an empty deque
4. Input r (number of elements to add to the deque)
5. Repeat r times:
   a. Input an integer
   b. Append it to the deque
6. Display "Stack before rotation" and the deque
7. Rotate the deque by n steps using rotate(n)
8. Display "Stack after rotation" and the rotated deque
9. End

### Program: 

```python
# Name: Nidhish B
# Reg.No: 212223050032

import collections
def fun(n):
    de=collections.deque([])
    r=int(input())
    for i in range(r):
        de.append(int(input()))
    print('Stack before rotation',de)
    de.rotate(n)
    print('Stack after rotation',de)
    
```
### Output:

![image](https://github.com/user-attachments/assets/b532bf85-e945-4a42-8bd3-f4ff0df7ddf2)

### Result:

Thus, the given program is implemented and executed successfully.
 


EX: 10.3 QUEUE
### Aim: 

To Develop a python program to remove the last 3 values from the queue.

### Algorithm:

1. Start
2. Initialize an empty list q
3. Input an integer n (number of elements to be added to the list)
4. Repeat the following n times:
    a. Input an integer x
    b. Append x to the list q
5. Repeat the following 3 times:
    a. Remove the last element of the list q using pop()
6. Display the updated list q
7. End

### Program:
```python
# Name: Nidhish B
# Reg.No: 212223050032

q=[]
n=int(input())

for i in range(n):
    q.append(int(input()))

for i in range(3):    
    q.pop()
print(q)
```

### Output:
![image](https://github.com/user-attachments/assets/fe9452ee-ba38-415b-b61b-8373f9852608)

### Result:
Thus,the given program is implemented and executed successfully.


### EX: 10.4 IMPLEMENTATION OF QUEUE

### Aim: 

To Develop a python program to get the 4 integer values from user and display the values using multiprocessing library

### Algorithm:

1. Start
2. Create an empty queue `q` using multiprocessing.Queue
3. Repeat 4 times:
    a. Input an integer x
    b. Enqueue x into queue `q` using q.put(x)
4. Repeat 4 times:
    a. Dequeue an element from queue `q` using q.get()
    b. Print the dequeued element
5. End

### Program:

```python
# Name: Nidhish B
# Reg.No: 212223050032

from multiprocessing import Queue

q=Queue()

for i in range(4):
    q.put(int(input()))
    
for i in range(4):
    print(q.get())
```
### Output:

![image](https://github.com/user-attachments/assets/1c4c3741-ef9f-421d-8a39-0e2b098c6cfb)

### Result:

Thus,the given program is implemented and executed successfully.
 


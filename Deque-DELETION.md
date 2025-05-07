# Exp.No: 14D
## Deque - DELETION

---

### AIM  
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.

---

### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Create an empty deque.  
3. Define how many elements to input (e.g., 3 inputs as in the example).  
4. Loop through the range of input size:  
   - Read an integer from the user.  
   - Append the integer to the deque.  
5. Remove the front element of the deque using `popleft()`.  
6. Print the final deque after deletion.  

---

### PROGRAM  

import collections  <br />
n1=input()  <br />
n2=input() <br />
n3=input()  <br />

col=collections.deque([n1,n2,n3])  <br />

col.popleft() <br />

print("The deque after deletion is :") <br />
print(col)

### OUTPUT


![Screenshot 2025-05-07 112453](https://github.com/user-attachments/assets/b47a8bbc-95c6-4a1a-aec0-cfd5b4fceb43)


### RESULT

Thus , the given python program is implemented and executed sucessfully.

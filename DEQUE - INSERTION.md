# Exp.No:39  
## DEQUE - INSERTION



### AIM  
To write a Python program to insert elements at REAR END of deque using a collection built-in function.



### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Initialize an empty deque.  
3. Start an infinite loop using `while True`.  
4. In each iteration, take input from the user.  
5. If the input is an empty string, break the loop.  
6. If the input is not empty, convert it to an integer and append it to the deque.  
7. After the loop ends, append the values `14` and `15` to the deque.  
8. Print the message `"The deque after appending at right is :"`.  
9. Print the contents of the deque.  



### PROGRAM  

import collections   <br />
x=int(input())  <br />
y=int(input())  <br />
z=int(input())   <br />
de=collections.deque([x,y,z])   <br />
print("The deque after appending at right is :")   <br />
de.append(14)   <br />
de.append(15)  <br />
print(de)



### OUTPUT

![Screenshot 2025-05-07 111947](https://github.com/user-attachments/assets/eff176db-76f6-4435-88b7-00a27a88f21c)


### RESULT
Thus, the given python program is implemented and executed sucessfully.

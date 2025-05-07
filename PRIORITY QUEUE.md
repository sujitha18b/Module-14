# Exp.No: 14 E
## PRIORITY QUEUE

---

### AIM  
To write a Python program for simple implementation of Priority Queue using Queue.

---

### ALGORITHM

1. Start the program.  
2. Define a class `PriorityQueue` with an initializer to create an empty list `queue`.  
3. Define the `__str__` method to return queue elements as a string separated by spaces.  
4. Define the `isEmpty()` method to check if the queue is empty.  
5. Define the `insert(data)` method to append the given data to the queue.  
6. Define the `delete()` method to:  
   - Initialize `max_val` as 0.  
   - Loop through the queue and find the index of the maximum value.  
   - Delete and return the element at that index.  
7. In the main code, take integer input `n` for number of elements.  
8. Loop `n` times to take input values and insert them into the priority queue.  
9. Print the contents of the queue.  
10. While the queue is not empty, call `delete()` and print each returned element.  
11. End the program.

---

### PROGRAM

class PriorityQueue(object):  <br />
	def __init__(self):  <br />
		self.queue = [] <br />

def __str__(self):  <br />
		return ' '.join([str(i) for i in self.queue])  <br />

	
def isEmpty(self): <br />
		return len(self.queue) == 0  <br />

	
def insert(self, data):  <br />
	    self.queue.append(data)  <br />

	
def delete(self):  <br />
		try:  <br />
			max_val = 0 <br />
			for i in range(len(self.queue)): <br />
				if self.queue[i] > self.queue[max_val]: <br />
					max_val = i <br />
			item = self.queue[max_val] <br />
			del self.queue[max_val] <br />
			return item <br />
		except IndexError: <br />
			print() <br />
			exit() <br />


myQueue = PriorityQueue() <br />
n=int(input())	 <br />
for i in range(0, n): <br />
    ele = int(input()) <br />
    myQueue.insert(ele) <br />
	
print(myQueue)		 <br />
while not myQueue.isEmpty(): <br />
	print(myQueue.delete())

### OUTPUT


![Screenshot 2025-05-07 113126](https://github.com/user-attachments/assets/302915e1-1971-4692-9373-4ae8eb97497d)


### RESULT

Thus , the given python program is implemented and executed sucessfully.

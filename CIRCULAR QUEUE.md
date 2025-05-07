# Exp No: 14 B
## Circular Queue 

### AIM  
To write a Python program with a function to insert float values into a Circular Queue.



### ALGORITHM

1. Start  
2. Check if the Circular Queue is full  
   - If `size == max_size`, print `"Queue is full"` and exit the function  
3. If the queue is not full:  
   - Read the element to be inserted  
   - Convert it to float  
   - Insert the element at the `tail` position  
   - Update tail using: `tail = (tail + 1) % max_size` (circular increment)  
   - Increment `size` by 1  
4. End



### PROGRAM


class Queue:   <br />
    def __init__(self, size):  <br />
        self.items = [0] * size <br />
        self.max_size = size  <br />
        self.head, self.tail, self.size = 0, 0, 0  <br />

  def enqueue(self, item):  <br />
        if self.is_list_full():  <br />
            print("Queue is full")  <br />
            return <br />
        
  self.items[self.tail]=item <br />
        self.tail=(self.tail+1)%self.max_size <br />
        self.size+=1  <br />
            
   

   def is_list_full(self):  <br />
        if self.size==self.max_size:  <br />
            return True  <br />
        return False  <br />

 def is_empty(self): <br />
        if self.size==0: <br />
            return True  <br />
        return False <br />


size=int(input())  <br />
queue=Queue(size)  <br />
str=float(input())  <br />
str1=float(input())  <br />
str2=float(input())  <br />
queue.enqueue(str) <br />
queue.enqueue(str1) <br />
queue.enqueue(str2) <br />
print(queue.items)


### OUTPUT

![Screenshot 2025-05-07 111425](https://github.com/user-attachments/assets/571eafbd-4719-40e7-91a5-f7abc6173c0b)


### RESULT

Thus , the given python program is implemented and executed sucessfully.

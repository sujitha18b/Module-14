# Exp.No: 14 A
## APPLICATIONS OF QUEUE



### AIM  
To write a Python program to implement CPU Process Scheduling using a queue.



### ALGORITHM  

1. Start the program.  
2. Define the function `CalculateWaitingTime(at, bt, N)`.  
3. Initialize a list `wt` of size `N` with all values set to 0.  
4. Set `wt[0] = 0` for the first process.  
5. Print the table header: "P.No.", "Arrival Time", "Burst Time", "Waiting Time".  
6. Print the values for the first process.  
7. For each process from index `1` to `N-1`:  
   - Calculate `wt[i] = (at[i - 1] + bt[i - 1] + wt[i - 1]) - at[i]`.  
   - Print the process number, arrival time, burst time, and waiting time.  
8. Initialize `total_waiting_time = 0`.  
9. Add up all waiting times.  
10. Calculate average waiting time as `average = total_waiting_time / N`.  
11. Print the average waiting time.  
12. Get burst times as input from the user for 5 processes.  
13. Call `CalculateWaitingTime()` with `at`, `bt`, and `N`.  
14. End the program.


### PROGRAM  

def CalculateWaitingTime(at, bt, N): <br />


wt = [0]*N; <br />

wt[0] = 0; <br />

print("P.No.\tArrival Time\t" , "Burst Time\tWaiting Time"); <br />
	print("1" , "\t\t" , at[0] , "\t\t" , bt[0] , "\t\t" , wt[0]); <br />


for i in range(1,5): <br />
		wt[i] = (at[i - 1] + bt[i - 1] + wt[i - 1]) - at[i]; <br />

print(i + 1 , "\t\t" , at[i] , "\t\t" , bt[i] , "\t\t" , wt[i]); <br />
	

sum = 0; <br />

	
for i in range(5): <br />
		sum = sum + wt[i]; <br />
	

average = sum / 5; <br />

	
print("Average waiting time = " , average); <br />



N = 5; <br />

	
at = [ 0, 1, 2, 3, 4 ]; <br />

	
bt=[] <br />
for i in range(0, 5): <br />
    ele = int(input()) <br />
    bt.append(ele) <br />
	

	
CalculateWaitingTime(at, bt, N); 


### OUTPUT

![Screenshot 2025-05-07 110305](https://github.com/user-attachments/assets/8451b385-feba-4ad6-8a7b-ceaaea487723)


### RESULT
 Thus , the given python program is implemented and executed sucessfully.

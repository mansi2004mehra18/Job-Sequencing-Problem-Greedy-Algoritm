# Job-Sequencing-Problem-Greedy-Algoritm

Job Sequencing Problem
Given an array of jobs where every job has a deadline and profit if the job is finished before the deadline. It is also given that every job takes a single unit of time, so the minimum possible deadline for any job is 1. Maximize the total profit if only one job can be scheduled at a time.

Jobs Given:
Job A = (Deadline: 4, Profit: 20)
Job B = (Deadline: 1, Profit: 10)
Job C = (Deadline: 1, Profit: 40)
Job D = (Deadline: 1, Profit: 30)
Solution Approach:
Answer: C, A
Time = 1, Profit = 40
Time = 2, Profit = 40 + 20 = 60
Alternative Scheduling:

Time = 2, Profit = 30 + 20 = 50
Using a Greedy Algorithm, the optimal solution schedules Job C first (highest profit for time = 1), followed by Job A (since its deadline allows it to be scheduled next).

Approach
1️⃣ Sort jobs based on Profit

2️⃣ Initialize time = 0

cpp
Copy
Edit
for(int i = 0; i < jobs; i++) {
    if (job(deadline) > time) {
        add job in ans  
        time++
    }
}
Time Complexity: 
𝑂
(
𝑛
×
2
)
O(n×2)
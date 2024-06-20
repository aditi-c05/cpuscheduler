# Cpu Scheduler
In an operating system, the CPU scheduler is a crucial component responsible for determining which process gets to use the CPU and for how long. There are different types of CPU scheduling algorithms like First-Come, First-Served (FCFS), Shortest Job Next (SJN), Round Robin, Shortest Remaining Time , Highest response ratio next , Feedback and aging etc.

Each algorithm has its own way of selecting the next process to run. For example, the Round Robin algorithm assigns a fixed time slice to each process, allowing them to run for that duration before moving to the next process. This helps in sharing the CPU fairly among all processes.

Schedulers play a significant role in optimizing system performance by managing the execution of processes efficiently. They aim to reduce the waiting time of processes, improve system throughput, and ensure fairness in CPU allocation. 
# Dependencies of the project
the following are the dependencies-
1) Use of Standard C++ Library.
   #include <bits/stdc++.h>
2) Use of Custom Header.
   #include "parser.h"

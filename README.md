# Cpu Scheduler
In an operating system, the CPU scheduler is a crucial component responsible for determining which process gets to use the CPU and for how long. There are different types of CPU scheduling algorithms like First-Come, First-Served (FCFS), Shortest Job Next (SJN), Round Robin, Shortest Remaining Time , Highest response ratio next , Feedback and aging etc.

Each algorithm has its own way of selecting the next process to run. For example, the Round Robin algorithm assigns a fixed time slice to each process, allowing them to run for that duration before moving to the next process. This helps in sharing the CPU fairly among all processes.

Schedulers play a significant role in optimizing system performance by managing the execution of processes efficiently. They aim to reduce the waiting time of processes, improve system throughput, and ensure fairness in CPU allocation. 
# Dependencies of the project
the following are the dependencies-
1) Use of Standard C++ Libraries.
iostream
vector
queue
tuple
algorithm
cmath
2) Use of Global Constants and Variables
TRACE, SHOW_STATISTICS
ALGORITHMS
Printing Functions
Functions (printProcesses, printArrivalTime, printServiceTime, printFinishTime, printTurnAroundTime, printNormTurn, printStats, printTimeline) responsible for displaying process information, timeline visualization, and statistical summaries.

# How to Run the project
Ensure Dependencies:
Make sure you have a C++ compiler installed on your system (e.g., GCC , or Xcode for macOS).
Ensure that your compiler supports C++11 or later, as the code uses features from these standards (like std::tuple, std::vector, etc.).
Use of Text editors like Visual Studio Code.
Command Line Execution
After successful compilation, run the executable ..scheduler.

# Internal Working of the project
The project likely revolves around simulating various CPU scheduling algorithms and analyzing their performance based on process arrival times, burst times (service times), and scheduling policies.

Algorithm Implementation:

First-Come, First-Served (FCFS):
First Come First Served (FCFS) is a scheduling algorithm in which the process that arrives first is executed first. It is a simple and easy-to-understand algorithm, but it can lead to poor performance if there are processes with long burst times. This algorithm does not have any mechanism for prioritizing processes, so it is considered a non-preemptive algorithm. In FCFS scheduling, the process that arrives first is executed first, regardless of its burst time or priority. This can lead to poor performance, as longer running processes will block shorter ones from being executed. It is commonly used in batch systems where the order of the processes is important.

Shortest Job First (SJF): 
Shortest JOB FIRST (SJF) is a scheduling algorithm that prioritizes the execution of processes based on their burst time, or the amount of time they need to complete their task. It is a non-preemptive algorithm which means that once a process starts executing, it runs until completion or until it enters a waiting state.

The algorithm maintains a queue of processes, where each process is given a burst time when it arrives. The process with the shortest burst time is executed first, and as new processes arrive, they are added to the queue and sorted based on their burst time. The process with the shortest burst time will always be at the front of the queue, and thus will always be executed next.

This algorithm can be beneficial in situations where the objective is to minimize the average waiting time for processes, since shorter processes will be executed first, and thus will spend less time waiting in the queue. However, it can lead to longer running processes being blocked by shorter ones, which can negatively impact the overall performance of the system.

In summary, SJF is a scheduling algorithm that prioritizes the execution of processes based on their burst time, it's non-preemptive and it's commonly used in situations where the objective is to minimize the average waiting time for processes.

Round Robin (RR):
Round Robin (RR) with variable quantum is a scheduling algorithm that uses a time-sharing approach to divide CPU time among processes. In this version of RR, the quantum (time slice) is not fixed and can be adjusted depending on the requirements of the processes. This allows processes with shorter burst times to be given smaller quanta and vice versa.

The algorithm works by maintaining a queue of processes, where each process is given a quantum of time to execute on the CPU. When a process's quantum expires, it is moved to the back of the queue, and the next process in the queue is given a quantum of time to execute.

The variable quantum allows the algorithm to be more efficient as it allows the CPU to spend more time on shorter processes and less time on longer ones. This can help to minimize the average waiting time for processes. Additionally, it also helps to avoid the issue of starvation, which occurs when a process with a long burst time prevents other processes from executing.

Data Structures:

Queue or List: To maintain the order of processes based on arrival times or specific scheduling criteria.
Arrays or Vectors: For storing process attributes such as burst times, arrival times, and execution times.

Execution and Output:

During execution, record timeline events (like start and end times of processes).
Compute statistics like turnaround time (completion time - arrival time) and waiting time.
Depending on the operation mode (trace or stats), generate and display output:
Trace Mode: Visual timeline or sequence of events showing process execution.
Stats Mode: Summary statistics such as average turnaround time, average waiting time, etc.

# Learnings Takeaways from the project
Working on a CPU scheduling simulation project can provide several valuable learning takeaways, both in terms of technical skills and broader understanding of operating system principles. 

Technical Skills I Learn
> Understanding Scheduling Algorithms
> Data Structures Usage

Overall, working on a CPU scheduling simulation project is a hands-on way to deepen understanding of operating system concepts, improve programming skills, and develop critical analytical and problem-solving abilities. 

# Resources
The resources I used are-
https://www.youtube.com/playlist?list=PLBlnK6fEyqRitWSE_AyyySWfhRgyA-rHk(for learning differnt algos)

https://github.com/yousefkotp/CPU-Scheduling-Algorithms?tab=readme-ov-file#installation( for learning of implementation of different algorithms)


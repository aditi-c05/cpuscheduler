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
   
2) Use of Local Header.
   #include "parser.h"
3) Use of Global Constants and Variables
Constants: Strings TRACE and SHOW_STATISTICS, and ALGORITHMS array.
Global Variables: Arrays finishTime, turnAroundTime, normTurn, and timeline
# How to Run the project
Ensure Dependencies:
Make sure you have a C++ compiler installed on your system (e.g., GCC , or Xcode for macOS).
Ensure that your compiler supports C++11 or later, as the code uses features from these standards (like std::tuple, std::vector, etc.).

Project Setup:
Place all your source files (main.cpp, parser.h) in the same directory.

Compile the Project:

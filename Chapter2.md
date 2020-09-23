### Process Concept :-An abstraction og a running program.
"Resource Management"<---OS----> more than one program is currently running.

-Swapping between processes.
-Scopping:- 10ms or 100ms
-Architecture:-Impacts OS efficiency(It makes one OS from other)
-Process Control Block(PCB's)
*Data Structure that OS uses to keep track of each process.
*Swapping is Unpredicatable from the perspective of the program.
Scheduling:
->Trigger Rev
  -LACK OF RESOURCE
  -Priority
Process vs Program
-Process is a running program on the machine.
-Program is a series of instruction


Examples

Windows                                     Unix-related(OS)
Create Process                                BSD----(Max OS)
                                              Linux
                                              fork()(Keep track of parent and child process)
                                              (fork makes a copy of process and runs it)
Shell
->command,packages,flags[Fork execute]

Process States and Transition
1)ready State<-----------------------------
2)Running State------   <-----------|     |
                    | Request Resource    |
                    |                     |
3)Block state <------        --------------

Why Processes
-Because abstraction

Multiple processes are connected to a virtual CPU and the virtual CPU is connected to a CPU.

"Listless" implementation

** 2.4-2.6 **
-> Where do processes comes from
  *Bootstrapping
  -> Hardware can run a program(boot loader) to start loading the OS(process).
-> R.C.B
  * Resource Description                                                                                                                    
  * Availability------------------------------------------------------------->*Atomic   *Multiport(Multiple process can be served at once)
  * wait list->list of pointers of PCB's(array)
  
 #### Round Robin scheduling
 "Taking turns"
 ![](https://media.geeksforgeeks.org/wp-content/uploads/round-robin-1.jpg)
 #### Multi level scheduling algorithm
  ![](https://media.geeksforgeeks.org/wp-content/uploads/multilevel-queue-schedueling-1-300x217.png)
 
 #### Multilevel Feedback Scheduling
  ![](https://media.geeksforgeeks.org/wp-content/uploads/Multilevel-Feedback-Queue-Scheduling-300x269.png)
  Balance 
  > - Between prority
  > - not saturation
  
  ### Trade of balance throughput & quanta size
  #### Interactive Processes
  > - Recieve process
  > - process
  > - respond proces
  Larger Quanta and Small quant
 #Context Switching(Expansive)
 - Takes a sgnified amount of fine
 
 #### Worst case Scenario
 
 #### Large Quantum
 > - Size quantum increases
 
 
 #### Real Time Processes
 ##### done within a deadline
 > - airplane(fly-by-wire) and also cars(drive by wire)
 > - Streaming video or teleconference
 > - Period 
 > - runtime
 
 ### Rate Monotonic Scheduling
 #### shorter the period, higher the priority
 
 ### Earliest Deadline First(EDF)
 #### Shorter the remaining time, higher the priority
 
 **Feasable - Deadline for all processes can be met.**
 **3.5 Read**

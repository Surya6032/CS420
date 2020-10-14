## Deadlocks

2 process
2 resource

- 2 processes to play an audio file

Pl                                    p2
- request file                        - request soundcard
- request sound card                  - request file



![Image of deadlock](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2015/06/deadlock.png)


#### 4 Required conditions deadlock
1. Mutual Exclusion
2. Hold and wait
3. No Preemption
4. Circular Waiting

#### Resource Allocation Graph

![Image of allcation](https://media.geeksforgeeks.org/wp-content/uploads/Slide6-1.jpg)


Transitions that affect resource allocation graph
1. Request Resource 
  - only if not already blocked
  -Never req more resource than exist
2. Resource acquisition 
  - only allocated one resource at a time
3. Release a resource
  - must be running to release a resource
  - cannot release more resources than I was acquired
 
 


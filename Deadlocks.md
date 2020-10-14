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
 
#### Strategies:
1. Ignore the problem
2. Detect a deadlock - Recover
3. Avoid Deadlocks
4. Prevent Deadlocks
  -> Toddling 1 of the 4 requirements
####  System States
- Deadlocked State
- Safe State
#### Deadlock detection                    
-  Graph Reduction                          
  * Select and Unblocked Process             
  * Remove that Process
    - Remove all aquisation
    - if any reqests can be filled do so
#### Throrem 1: State S is deadlock if resoucrce graph not completely reducible
#### Theorem 2: All reduction sequences of a given resource allocation graph lead to the same final graph.

#### Continuos deadlock detection
Facts
- If the current state S is not deadlock 
  Then: Next state is deadlock only if 
    1) The operation that caused S ---> S' was a request
    2) must be that the requesting process is now involved in deadlock
- If the recent transition was a request
  1) only possible to have a deadlock if the requesting process is involved .
    Sufficient to graph reduce. ONLY until p is reduced
    
#### Deadlock avoidance
  - all processes report on "Maximum claim"
  - "resource allocation graph" 
  - "resource allocation matrices"
  
  - Process needs to know max resource its gonna ask for
  - Assumes:
    - States set of process
  

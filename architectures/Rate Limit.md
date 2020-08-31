# Rate Limit

##### Advantages of Rate Limit

- User Experience
- Security
- Operational Costs

##### Types of Rate Limit

- User Based 
- Concurrent (mitigate DDOS)
- Location/IP Based 
- Server Based 

##### Algorithms

- Token Bucket: User ID, Time Stamp and Counter

  ![Token Bucket](/images/Token_Bucket.png)

- Leaky Bucket: FIFO Used as Queue. 

  ![Leaky Bucket](\\System-Design\images\Leaky_Bucket.png)

- Fixed Window Counter: 

  ![Fixed Window Counter](\\System-Design\images\Fixed_Window_Counter.png)

- Sliding Logs: 

  ![](\\System-Design\images\Sliding_Window_Counter.png)

- Sliding Window Counter: With Counter 

##### Problems and Concerns 

- Inconsistency: Sticky Session (Always use same Load Balancer) 
- Race Condition: Locks
  - Relaxing Rate Limit
  - Local Memory Async at rate limiter. 

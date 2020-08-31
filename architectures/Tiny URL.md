# Tiny URL

##### Data Capacity Model 

- Long URL : 2 KB 
- Short URL: 17 Bytes
- Created at: 7 Bytes
- Expiration at: 7 Bytes
- Total: 2.031 KB/Entry in the Table.

##### Character Random ID Generator

- B62 
  - A-Z,a-z,0-9 
  - 62^7 : 3.5 Trillion 

- MD5

##### Database Selection

- RDBMS
  - ACID
  - Problems: Scaling
- NoSQL
  - Scaling

##### Solution Techniques

- Database Read and Writes (Put if absent)
- MD5 approach (Put if absent)
- Using Counters.

##### Zookeeper

- Distributed coordination service.

 ![Distributed URL Shortner using Zoo Keeper](/images/Zoo_Keeper.png)

##### APIs

- createTinyURL 
- getLongURL 
- Analytics
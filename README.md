## Tapestry Algorithm
	
## Project compiled by
	Akash Jajoo
	Niraj Chowdhary

## Steps to execute
1. Extract Tapestry_Algorithm to you local machine
2. Go to Project 3/tapestry folder via command prompt
3. Type **mix run proj3.exs arg1 arg2** 
  Here,
     **arg1** is the number of nodes involved
      **arg2** Number of request per node.  
    **Output:**  Maximum number of hops taken to find the requested file.
    
 
## Tapestry algorithm
1. Here every node in the network has their own 16 bit long identifier
2. Each node maintains a finger table which is the key value pair, just like hash map, that points to the neighbours it knows about.
3. Neighbour is selected on basis of prefix matching, whichever has the longest prefix matching is chosen as the next node to hop to.
4. The above proecess continues until desired object is found and it takes O(logn) time.


## Output:
[![Annotation-2020-01-24-215737.png](https://i.postimg.cc/XYnBWK5w/Annotation-2020-01-24-215737.png)](https://postimg.cc/7fQZM2m6)


The above screenshot demonstrates the working output of 100 and 1000 nodes handling 2 requests and 4 request per node respectively.
For 100 nodes the maximum no. of hops is 2 to find an object and for 1000 nodes it is 4.

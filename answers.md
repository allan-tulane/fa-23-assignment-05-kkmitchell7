# CMPS 2200 Assignment 5
## Answers

**Name:** Kailen Mitchell






- **1a.**

Maximum depth where n is number of items and d is the number of comparisons needed
ℎ=⌈log𝑑(𝑛𝑑−𝑛+1)⌉−1


- **1b.**

Work where n is number of items and d is the number of comparisons needed:

Delete min: O(d*log_d(n))

Insert: O(log(n)/log(d))

- **1c.**

V = number of verticies
E = number of edges
d = degree of d-ary heap

Work: O((V + E) * d * logd(V))

account for delete min and insert seperately?


- **1d.**


d = V^(log(V))


- **2a.**

APSP(0,1,0) = -2
APSP(0,2,0) = 2
APSP(1,2,0) = 0

APSP(0,1,1) = -2
APSP(0,2,1) = -1
APSP(1,2,1) = 0

APSP(0,1,2) = -2
APSP(0,2,2) = -1
APSP(1,2,2) = 0

- **2b.**

The relationship between APSP(i,j,1) and APSP(i,j,2) is that they are the same.

APSP(i,j,2) = APSP(i,j,1)

write in terms of  APSP(i,j,0) as well?

- **2c.**

The shortest path is always APSP(i,j,k-1)

give an optimal substructure property?

- **2d.**

n^3 distinct subproblems will be computed

The work of this dynamic programming algorithm is O(n^3)


- **2e.**

Work of Johnson's: O((V + E) * d * logd(V))
This one: O(n^3)

which is worse?

- **3a.**

No because the MST algorithm doesn't inherently minimize the maximum edge weights since it greedily selected edges with the smallest weights while ensuring the tree is still valid.


- **3b.**


First, compute the MST
Next, store all the edges of the MST
Next, iterate through each edge and recalculate the MST without the edge
Finally, select the next best tree amoung the trees just obtained



- **3c.**

Work: O(VE)
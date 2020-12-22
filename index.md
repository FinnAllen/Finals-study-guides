# HW 1

**6.1**


1) What are the minimum and maximum numbers of elements in a heap of height hh?


2) Show that an n-element heap has height \lfloor \lg n \rfloor⌊lgn⌋.


7) Show that, with the array representation for sorting an n-element heap, 
the leaves are the nodes indexed by \lfloor n / 2 \rfloor + 1, \lfloor n / 2 \rfloor + 2, \ldots, n⌊n/2⌋+1,⌊n/2⌋+2,…,n.


**6.2**


3) What is the effect of calling MAX-HEAPIFY(A, i) when the element 
A[i] is larger than its children?


4) What is the effect of calling MAX-HEAPIFY(A, i) for i > A.heap/2?


5) The code for \text{MAX-HEAPIFY}MAX-HEAPIFY is quite efficient in
terms of constant factors, except possibly for the recursive call in
line 10, which might cause some compilers to produce inefficient code.
Write an efficient MAX-HEAPIFY that uses an iterative control construct
(a loop) instead of recursion.


**6.5**


8) write heap-delete that runs in O(logn) time


9) Give an O(n\lg k)O(nlgk)-time algorithm to merge kk sorted lists
into one sorted list, where nn is the total number of elements in all
the input lists. Hint: Use a min-heap for k-way merging.)


#HW 2

**§2.3**


2) Rewrite the MERGE procedure so that it does not use sentinels,
instead stopping once either array LL or RR has had all its elements
copied back to AA and then copying the remainder of the other array
back into A.


3) show the solution to the recurance when n is an exact power of 2 is
T(n) = nlgn


4) We can express insertion sort as a recursive procedure as follows. 
In order to sort A[1..n], we recursively sort A[1..n - 1] and then insert 
A[n] into the sorted array A[1..n - 1] Write a recurrence for the running
time of this recursive version of insertion sort.


5) Write binary search and argue it is lgn


7) describe an nlgn algorithm that, given a set S of nn integers and another
integer x, determines whether or not there exist two elements in S whose sum
is exactly x.


**7.2**


1)Use the substitution method to prove that the recurrence 
T(n) = T(n - 1) + Θ(n)T(n)=T(n−1)+Θ(n) has the solution T(n) = Θ(n^2)T(n)=Θ(n^2)
as claimed at the beginning of section 7.2.


**7.3**


1) Why do we analyze the expected running time of a randomized algorithm and
not its worst-case running time?


**8.1**
1) What is the smallest possible depth of a leaf in a decision tree for a comparison sort?


3) Show that there is no comparison sort whose running time is linear for
at least half of the n! inputs of length n. What about a fraction of 1/n of
the inputs of length n? What about a fraction 1 /2^n?


4) binary desicion tree


**9.2**
3) Write an iterative version of RANDOMIZED-SELECT.


**9.3**
3) Show how quicksort can be made to run in O(nlgn) time in the worst case,
assuming that all elements are distinct.


5) Suppose that you have a "black-box" worst-case linear-time median subroutine.
Give a simple, linear-time algorithm that solves the selection problem for an
arbitrary order statistic. (partition array based on median)

#HW 3

**8.1**


4) Suppose that you are given a sequence of n elements to sort. The input sequence consists of n / k subsequences, each containing k elements. The elements in a given subsequence are all smaller than the elements in the succeeding subsequence and larger than the elements in the preceding subsequence. Thus, all that is needed to sort the whole sequence of length nn is to sort the kk elements in each of the n / kn/k subsequences. Show an \Omega(n\lg k)Ω(nlgk) lower bound on the number of comparisons needed to solve this variant of the sorting problem. (\textit{Hint:}Hint: It is not rigorous to simply combine the lower bounds for the individual subsequences.)


**9.2**


3) Write an iterative version of RANDOMIZED-SELECT.


**9.3**


3) Show how quicksort can be made to run in O(nlgn) time in the worst case, assuming that all elements are distinct.


5) Suppose that you have a "black-box" worst-case linear-time median subroutine. Give a simple, linear-time algorithm that solves the selection problem for an arbitrary order statistic.


**21.3**


1) Redo Exercise 21.2-2 using a disjoint-set forest with union by rank and path compression.


2) Write a nonrecursive version of FIND-SET with path compression.


3) Give a sequence of m MAKE-SET, UNION, and FIND-SET operations, n of which are MAKE-SET operations, that takes Ω(mlgn) time when we use union by rank only.


4) Suppose that we wish to add the operation PRINT-SET(x), which is given a node x and prints all the members of x's set, in any order. Show how we can add just a single attribute to each node in a disjoint-set forest so that PRINT-SET(x) takes time linear in the number of members of x's set and the asymptotic running times of the other operations are unchanged. Assume that we can print each member of the set in O(1) time.


**15.2**


2) Give a recursive algorithm MATRIX-CHAIN-MULTIPLY(A,s,i,j) that actually performs the optimal matrix-chain multiplication, given the sequence of matrices {A_1, A_2, ... ,A_n}, the s table computed by MATRIX-CHAIN-ORDER, and the indices ii and jj. (The initial call would be MATRIX-CHAIN-MULTIPLY(A,s,1,n).)


4) Describe the subproblem graph for matrix-chain multiplication with an input chain of length n. How many vertices does it have? How many edges does it have, and which edges are they?




#HW 4

**15.4**


2) Give pseudocode to reconstruct an \text{LCS}LCS from the completed cc table and the original sequences X = (x_1, x_2, ... x_m) and Y = (y_1, y_2, ..., y_n) in O(m + n)O(m+n) time, without using the bb table.


5) Give an O(n^2) time algorithm to find the longest monotonically increasing subsequence of a sequence of nn numbers.



**§16.1**


2) Suppose that instead of always selecting the first activity to finish, we instead select the last activity to start that is compatible with all previously selected activities. Describe how this approach is a greedy algorithm, and prove that it yields an optimal solution.


3) Not just any greedy approach to the activity-selection problem produces a maximum-size set of mutually compatible activities. Give an example to show that the approach of selecting the activity of least duration from among those that are compatible with previously selected activities does not work. Do the same for the approaches of always selecting the compatible activity that overlaps the fewest other remaining activities and always selecting the compatible remaining activity with the earliest start time.


**§16.2**


4) Professor Gekko has always dreamed of inline skating across North Dakota. He plans to cross the state on highway U.S. 2, which runs from Grand Forks, on the eastern border with Minnesota, to Williston, near the western border with Montana. The professor can carry two liters of water, and he can skate mm miles before running out of water. (Because North Dakota is relatively flat, the professor does not have to worry about drinking water at a greater rate on uphill sections than on flat or downhill sections.) The professor will start in Grand Forks with two full liters of water. His official North Dakota state map shows all the places along U.S. 2 at which he can refill his water and the distances between these locations.


The professor's goal is to minimize the number of water stops along his route across the state. Give an efficient method by which he can determine which water stops he should make. Prove that your strategy yields an optimal solution, and give its running time.


5) Describe an efficient algorithm that, given a set {x_1, x_2, ..., x_n} of points on the real line, determines the smallest set of unit-length closed intervals that contains all of the given points. Argue that your algorithm is correct.


**§16.3**


2) Prove that a binary tree that is not full cannot correspond to an optimal prefix code.


5) Prove that if we order the characters in an alphabet so that their frequencies are monotonically decreasing, then there exists an optimal code whose codeword lengths are monotonically increasing.

#HW 5

**§16.3**


3) What is an optimal Huffman code for the following set of frequencies, based on
the first 8 Fibonacci numbers?

Can you generalize your answer to find the optimal code when the frequencies are the first nn Fibonacci numbers?


6) Suppose we have an optimal prefix code on a set C = {0,1,…,n−1} of characters and we wish to transmit this code using as few bits as possible. Show how to represent any optimal prefix code on C using only 2n - 1 + n lg n \rceil2n−1+n⌈lgn⌉ bits. (Hint: Use 2n − 1 bits to specify the structure of the tree, as discovered by a walk of the tree.)


7) Generalize Huffman's algorithm to ternary codewords (i.e., codewords using the symbols 0, 1, and 2), and prove that it yields optimal ternary codes


9) Show that no compression scheme can expect to compress a file of randomly chosen 8-bit characters by even a single bit. (Hint: Compare the number of possible files with the number of possible encoded files.)


#HW 6

**§22.1**


1) Given an adjacency-list representation of a directed graph, how long does it take to compute the out-degree of every vertex? How long does it take to compute the in-degrees?


3) The transpose of a directed graph G = (V, E) is the graph G^T = (V, E^T). Thus G^T is G with all of it's edges reversed 


4) Given an adjacency-list representation of a multigraph G = (V, E), describe an O(V + E)-time algorithm to compute the adjacency-list representation of the "equivalent" undirected graph G' = (V, E') consists of the edges in EE with all multiple edges between two vertices replaced by a single edge and with all self-loops removed.


5) if and only if G contains a path with at most two edges between u and v. 


**§23.1**


1) Let (u, v) be a minimum-weight edge in a connected graph G. Show that (u, v) belongs to some minimum spanning tree of G.


3) Show that if an edge (u, v) is contained in some minimum spanning tree, then it is a light edge crossing some cut of the graph.


**§23.2**


1) Kruskal's algorithm can return different spanning trees for the same input graph G, depending on how it breaks ties when the edges are sorted into order. Show that for each minimum spanning tree T of G, there is a way to sort the edges of G in Kruskal's algorithm so that the algorithm returns T.


2) Suppose that we represent the graph G = (V, E) as an adjacency matrix. Give a simple implementation of Prim's algorithm for this case that runs in O(V^2) time.


**§24.3**


6) We are given a directed graph G = (V, E) on which each edge (u, v) in E has an associated value r(u, v), which is a real number in the range 0 ≤ r(u, v) ≤1 that represents the reliability of a communication channel from vertex u to vertex v. We interpret r(u, v) as the probability that the channel from u to v will not fail, and we assume that these probabilities are independent. Give an efficient algorithm to find the most reliable path between two given vertices.

# HW 7

**§25.1**


2) Why do we require that w_{ii} = 0 for all 1 <= i <= n?


4) Show that matrix multiplication defined by EXTEND-SHORTEST-PATHS is associative.


5) Show how to express the single-source shortest-paths problem as a product of matrices and a vector.


6) Suppose we also wish to compute the vertices on shortest paths in the algorithms of this section. Show how to compute the predecessor matrix ∏ from the completed matrix L of shortest-path weights in O(n^3) time.


7) We can also compute the vertices on shortest paths as we compute the shortest path weights. Define π_ij^(m) as the predecessor of vertex j on any minimum-weight path from i to j that contains at most m edges. Modify the EXTEND-SHORTESTPATHS and SLOW-ALL-PAIRS-SHORTEST-PATHS procedures to compute the matrices as the matrices {L^(1), L^(2), .., L^(n - 1)} are computed.


8) The FASTER-ALL-PAIRS-SHORTEST-PATHS procedure, as written, requires us to store ⌈lg(n−1)⌉ matrices, each with n^2 elements for a total space requirement of Θ(n^2 lg n). Modify the procedure to require only Θ(n^2) space using only n x n matrices. 


**§25.2**


4) As it appears above, the Floyd-Warshall algorithm requires Θ(n^3) space, since we compute d_{ij}^(k) for i, j, k = 1, 2 , … , n. Show that the following procedure, which simply drops all the superscripts, is correct, and thus only Θ(n^2) is required. 
























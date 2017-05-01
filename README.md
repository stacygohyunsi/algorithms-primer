# algorithms-primer
A consolidated collection of resources for you to learn and understand algorithms and data structures easily. 

# Objectives
It is difficult to find consolidated resources on algorithms. 
This repo hopes to gather resources to help one understand algorithms better to prepare 
for technical tests or simply to strengthen your foundation of computer science to help you become a better coder.

# Contributions
Contributions are more than welcome. I cant do everything myself, so I will need all the help I can get. To 
- add a new section or to 
- add on to existing sections, 
- or translate
simply submit a pull request. 

If you are arent sure of how to create a pull request, view the [pull request documentation](https://help.github.com/articles/about-pull-requests/).

# Algorithms Topics
Summaries of the algorithms topics:

### Brute force method
Brute force is simplest way to explore the space of solutions - simply means to go through all solutions, however unlikely they may be, something which is not particularly elegant.

## Dynamic Programming (DP)
What is DP?
DP or dynamic optimization basically means to take our problem and somehow break it down into
a reasonable number of subproblems so that we can use optimal solutions to the smaller subproblems to give us optimal solutions to the larger ones.

- Allows solve many different types of problems in time O(n)^2 or O(n)^3
- Usually focused on Principle of Optimality, "An optimal solution to any instance of an optimization problem is composed of optimal solutions to its subinstances"

Read more here:
Competitive Programming book by Steven and Felix Halim
http://www.techiedelight.com/introduction-dynamic-programming/

Practice here: 
https://www.hackerrank.com/domains/algorithms/dynamic-programming

### Memoization vs Tabulation
Memoization is an optimization technique used primarily to speed up computer programs by storing the results of expensive function calls and returning the cached result when the same inputs occur again. 

Which is better?


### Greedy Algorithms 
In greedy algorithm approach, it builds up a solution piece by piece, where the next piece that offers the most obvious and immediate benefit is chosen.

Algorithms which use the greedy approach:
- Travelling Salesman Problem
- Prim's Minimal Spanning Tree Algorithm
- Kruskal's Minimal Spanning Tree Algorithm
- Dijkstra's Minimal Spanning Tree Alsgorithm
- Graph - Map Coloring
- Graph - Vertex Cover
- Knapsack Problem
- Job Scheduling Problem 

**Common interview questions:**
- 0/1 Knapsack Problem
- Coin change - Given a set of coins and amount, Write an algo­rithm to find out how many ways we can make the change of the amount using the coins given.
- Edit Distance - Given two strings and a set of operations Change (C), insert (I) and delete (D) , find minimum number of edits (operations) required to transform one string into another.
- Longest Common Subsequence

### Knapsack problem with Repetitions
Knapsack problem or the rucksack problem is part of dynamic programming and it is where given a set of items, each with a weight and a value, determine the number of each item to include in a collection so that the total weight is less than or equal to a given limit and the total value is as large as possible. 

Read more: 
https://www.youtube.com/watch?v=8LusJS5-AGo (Introduction to Knapsack)
http://cse.unl.edu/~goddard/Courses/CSCE310J/Lectures/Lecture8-DynamicProgramming.pdf

Practice here: 
https://www.hackerrank.com/challenges/unbounded-knapsack

### Knapsack problem without Repetitions

# Data Structure
## Linked Lists

Introduction to linked lists/ Vectors vs. Linked List: https://www.youtube.com/watch?v=pBrz9HmjFOs (13 minute video)

- Link − Each link of a linked list can store a data called an element.

- Next − Each link of a linked list contains a link to the next link called Next.

- LinkedList − A Linked List contains the connection link to the first link called First.

[insert tutorial point image here]

- Linked List contains a link element called first.

- Each link carries a data field(s) and a link field called next.

- Each link is linked with its next link using its next link.

- Last link carries a link as null to mark the end of the list.

### Advantages/disadvantages of arrays vs linked lists
The linked lists have pointers to the next and the previous item unlike arrays.
**Advs of Linked Lists**
- Dynamic size
- Less expensive to insert/delete
	In arrays, you will have to shifts the items each time an items is inserted/deleted. For linked lists, you just have to change the links to point to the items.

**Disadvs of Linked Lists** 
- We cannot perform a random access of items. We have to access elements sequentially starting from the first node (or at the last node if it is a doubly linked list). So we cannot do binary search with linked lists. In arrays, however, you can simply specify the index of the array to get to the item.
- Extra memory space for a pointer is required with each element of the list.
- Arrays have better cache locality that can make a pretty big difference in performance.

### Applications of a linked list
Implementation of a stack/queue

### Single Linked List 
Item navigation is forward only

//insert single linked list diagrams

### Doubly Linked List
Items can be navigated forward and backward

//insert double linked list diagrams

### Circular Linked List 
In a circular singly linked list, the last node of the list is made to point to the first node.

### Operations on a Linked List
Insertion − Add a new data item in the given collection of data items.

Deletion − Delete an existing data item from the given collection of data items.
Traversal − Access each data item exactly once so that it can be processed.
Searching − Find out the location of the data item if it exists in the given collection of data items.
Sorting − Arranging the data items in some order i.e. in ascending or descending order in case of numerical data and in dictionary order in case of alphanumeric data.

Read more here: 

**Common interview questions**:

- Reverse a Linked List (recursive)
- Reverse a Linked List (iterative)
- Detect Loop in a Linked List
- Given pointers to two single-linked list, find out if they intersect and at which node they intersect
- Merge two unsorted linked list in efficient way
- Delete repeated elements from linked list

**Practice here**: 
https://www.hackerrank.com/domains/data-structures/linked-lists


### Queues

[insert image here: http://www.stoimen.com/blog/wp-content/uploads/2012/06/2.-Queue-Operations.png]
source: http://www.stoimen.com/blog/2012/06/05/computer-algorithms-stack-and-queue-data-structure/ 

Queues is a data structure which follows a First-In-First-Out (FIFO) or Last-In-Last-Out (LILO) methodology. 
One end is always used to insert data (enqueue) and the other is used to remove data (dequeue).

### Stacks

[insert image here: http://www.stoimen.com/blog/wp-content/uploads/2012/06/1.-Stack-Operations.png]
source: http://www.stoimen.com/blog/2012/06/05/computer-algorithms-stack-and-queue-data-structure/

Stacks is a data structure which follows a LIFO (last in, first out) methodology.	

To insert an item, it is called “Push”, to remove an item off is called “Pop”.

### Heaps

### Tree Traversal
### Deque

# Asymptotic notation
## Big-O Notation 
The Big O notation describes the complexity of an algorithm. 
It describes:
- The worst-case scenario, 
- the execution time required/space used
- the upper asymptotic bound

**O(1)**
- Same time regardless of the size of the input data

Coding examples:
- Accessing Array Index (int a = array[0];)
- print "hello";


**O(N)**
Performance will grow linearly and in direct proportion to the size of the input data set.

Coding examples: 
- Traversing an array
- Traversing a linked list
- Linear Search

**O(N)^2**
Performance is directly proportional to the square of the size of the input data set.
This is common with nested iterations over the data set.

These ones are supposed to be the less efficient algorithms if their O(n log n) counterparts are present.

Coding examples: 
- Bubble Sort
- Insertion Sort
-	 Selection Sort

**O(2N)**
Performance doubles with each additon to the input data set. The growth curve of an O(2N) function is exponential.

Coding examples: 
recursive calculation of Fibonacci numbers

**O(log n)**
O(log n) is slightly more difficult to explain. 
One good example of a O(log n) problem is when searching up a phone book. Even if the phone book is thick, you would not need to search every name, but you just have to look for the name under the correct alphabet. 

educing the problem size with every iteration

Coding examples:
- Binary search
- Finding largest/smallest number in a binary search tree

**O(n log n)**
To better understand it, think of it as O(N) and O(log n). An example of such a notation is the Quick sort when we divide the array into two parts and each time it takes O(N) time to find a pivot element. 

Coding examples:
- Merge Sort
- Heap Sort
- Quick Sort

## Big-Ω (Big-Omega) notation
- the lower asymptotic bound

## Big-θ (Big-Theta) notation
- Both the lower and upper asymptotic bound

# Search
## Linear Search
## Binary Search
## Naïve Divide and Conquer
## Breadth first search

# Sorting
## Bubble sort
## Selection sort
## Insertion sort
## Quick sort
## Merge sort

# Recursion
## Towers of Hanoi

# Graph Representation

# Travelling Salesman Problem

#Credits
I myself have learnt a lot while compiling these resources. Thanks to:
- [Hackerrank](https://www.hackerrank.com) 
- https://www.cs.cmu.edu/~avrim/451f09/lectures/lect1001.pdf
- Introduction to the Design & Analysis of Algorithms
- Quora
- Wikipedia
- http://algorithms.tutorialhorizon.com/dynamic-programming-coin-change-problem/
- https://www.tutorialspoint.com
- https://www.youtube.com/watch?v=pBrz9HmjFOs
- http://www.geeksforgeeks.org/linked-list-vs-array/
- https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation/

Inspired by:
https://github.com/donnemartin/system-design-primer#step-1-review-the-scalability-video-lecture

# Contact
I would really like to learn from you, so contact me for any issues or questions or ideas.
My github page is [here](https://github.com/stacygohyunsi) and my email is hello@imstacy.com

#License
```
Creative Commons Attribution 4.0 International License (CC BY 4.0)

http://creativecommons.org/licenses/by/4.0/
```






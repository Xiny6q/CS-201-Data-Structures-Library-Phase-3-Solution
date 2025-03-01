Download link :https://programming.engineering/product/cs-201-data-structures-library-phase-3-solution/

# CS-201-Data-Structures-Library-Phase-3-Solution
CS 201 Data Structures Library Phase 3 Solution
Phase 3 of the CS201 programming project, we will be built around heaps. In particular, you should implement both a standard binary heap and binomial heap. You will implement a class for each heap type.

You should create a class named Heap for the binary heap with public methods including the following (elmtype and valuetype are types from the template). You should use your dynamic array class for the heap storage.

Function

Description

Runtime

Heap();

Default Constructor. The Heap should be empty

O(1)

Heap(keytype k[], valuetype V[], int

For this constructor the heap should be built

O(s)

s);

using the arrays K and V containing s items of

keytype and valuetype. The heap should be

constructed using the O(n) bottom up heap

building method.

~Heap();

Destructor for the class.

O(1)

keytype peakKey();

Returns the minimum key in the heap without

O(1)

modifiying the heap.

valuetype peakValue();

Returns the value associated with the minimum

O(1)

key in the heap without modifiying the heap.

keytype extractMin();

Removes the minimum key in the heap and

O(lg n)

returns the key.

void insert(keytype k, valuetype v);

Inserts the key k and value v pair into the heap.

O(lg n)

void printKey()

Writes the keys stored in the array, starting at the

O(n)

root.

Your class should include proper memory management, including a destructor, a copy constructor, and a copy assignment operator.

You should create a class named BHeap for the binomial heap with public methods including the following (elmtype and valuetype are types from the template). You should use dynamic allocation for the binomial trees.

Function

Description

Runtime

BHeap();

Default Constructor. The Heap should be empty

O(1)

BHeap(keytype k[], valuetype V[],

For this constructor the heap should be built

O(s)

int s);

using the arrays K and V containing s items of

keytype and valuetype. The heap should be

constructed using repeated insertion.

~BHeap();

Destructor for the class.

O(n)

keytype peakKey();

Returns the minimum key in the heap without

O(lg n)

modifiying the heap.

valuetype peakValue();

Returns the value associated with the minimum

O(lg n)

key in the heap without modifiying the heap.

keytype extractMin();

Removes the minimum key in the heap and

O(lg n)

returns the key.

void insert(keytype k, valuetype v);

Inserts the key k and value v pair into the heap.

O(lg n)

void merge(BHeap<keytype,

Merges the H2 into the current heap

O(lg n)

valuetype> H2);

void printKey()

Writes the keys stored in the heap, printing the

O(n)

smallest binomial tree first. When printing a

binomial tree, print the size of tree first and then

use a modified preorder traversal of the tree.

See the example below.

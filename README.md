# CombinatorialIteration.m2
### CombinatorialIteration package for Macaulay2

### Iterative generators for combinatorial objects

*CombinatorialIteration*
is a package for generating combinatorial objects including 
partitions, permutations, subsets, and standard tableaux.
Objects are generated one by one: enter in an object to get the next one.

The primary purpose is to traverse a list of
partitions, permutations, subsets, or tableaux
without generating and storing the full list.
This arises in, for example, sums indexed by partitions;
iteration allows one to compute the terms of the sum one-by-one
by initializing a variable with the first partition
and repeatedly (with a for loop) iterating
the 'next' function to visit all of the partitions
exactly once each.

One may also go backward with 'prev[ious]' functions,
reversing the order of traversal of the 'next' functions.


### References
[NW]
: Nijenhuis, Albert; Wilf, Herbert S.
    *Combinatorial algorithms*.
    Second edition. 1978.

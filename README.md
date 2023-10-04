# Quiz 4

## Question 1: CamelCase

This algorithm runs in $O(n)$ because it is a single simple loop over the input.

This algorithm has linear space complexity. The input space has linear complexity. The auxiliary space is constant because the algorithm uses only one variable. Although Java's `toCharArray` method performs copying of the input, this is an implementation detail-- the algorithm would be equivalent if `charAt` was used, which does not perform any copying.

## Question 2: Correctness & Invariant 

The issue with the provided selection sort algorithm was that it did not properly sort the first item: i.e. swapping stopped at the *second* index instead of the first. 

This algorithm runs in $O(n^{2})$. The inner `while` loop may be converted to a `for` loop over `j = i down to 0`, which is mathematically represented as $\sum_{i=0}^{|A|} \sum_{j=0}^{i-1}1 = \sum_{i=0}^{|A|}i= \frac{|A|(|A| + 1)}{2} = O(n^{2})$.

The space complexity is linear for total complexity. It is linear for input space; it is constant for auxiliary space (as all variables may be hoisted to the outermost scope), so the linearity dominates for the overall space complexity.
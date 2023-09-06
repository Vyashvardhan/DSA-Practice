# DSA-Practice #
## Day 1: ##
  #### [Leetcode 283: Move Zeroes](https://leetcode.com/problems/move-zeroes/) ####
  Question: Given an integer array nums, move all 0's to the end of it while maintaining the relative order of the non-zero elements.
  - Topic: *Array*
  - Difficulty: *Easy*
  - Approach: Take two pointers(one for zero and the other for non-zero elements) and iterate through the array, whenever a zero is encountered by zeroth pointer stop iterating for that pointer and continue iterating for the other till a non-zero element is encountered or the last element of the array is reached, if non zero encountered then swap while end loop if last element reached.

   #### [LeetCode 453 - Max Consecutive Ones](https://leetcode.com/problems/max-consecutive-ones/) ####
   Question: Given a binary array nums, return the maximum number of consecutive 1's in the array.
   - Topic: *Array*
   - Difficulty: *Easy*
   - Approach: Keep two counters equal to zero and iterate through the array. if one is encountered then increase counter1, else set counter1 to zero. Before the end of each loop set counter2 as the maximum of both the counters.

   #### [LeetCode 73 - Set Matrix Zeroes]([https://leetcode.com/problems/max-consecutive-ones/](https://leetcode.com/problems/set-matrix-zeroes/)) ####
   Question: Given an m x n integer matrix matrix, if an element is 0, set its entire row and column to 0's.
   - Topic: *Array*
   - Difficulty: *Medium*
   - Approach: Initialise a column0 variable to 1. Iterate through the matrix, if element is zero then mark the 0th index of the row as zero and mark the column as zero if the column in not zero else mark the variable column0 as 0. Exit the loop. Run through the matrix again and changed the marked column and row to zero, except the 0th column and row. Exit the loop. Next, if the (0,0) index is zero then mark 0th row to zero. Similarly, if the variable column0 is zero, then mark the 0th column as zero.

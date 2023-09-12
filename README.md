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

   #### [LeetCode 73 - Set Matrix Zeroes](https://leetcode.com/problems/set-matrix-zeroes/) ####
   Question: Given an m x n integer matrix matrix, if an element is 0, set its entire row and column to 0's.
   - Topic: *Array*
   - Difficulty: *Medium*
   - Approach: Initialise a column0 variable to 1. Iterate through the matrix, if element is zero then mark the 0th index of the row as zero and mark the column as zero if the column in not zero else mark the variable column0 as 0. Exit the loop. Run through the matrix again and changed the marked column and row to zero, except the 0th column and row. Exit the loop. Next, if the (0,0) index is zero then mark 0th row to zero. Similarly, if the variable column0 is zero, then mark the 0th column as zero.

## Day 2: ##
#### [LeetCode 35 - Search Insert Position](https://leetcode.com/problems/search-insert-position/) ####
   Question: Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it would be if it were inserted in order.
   - Topic: *Binary Search*
   - Difficulty: *Easy*
   - Approach: Initialise a start, end and a result variable and iterate through the start to end of the array according to the binary search algorithm and search for the different element index and if the element is not found chexk if the element is greater or lesser than the element and change the start and end variable values accordingly while also searching for the position; also update the ressult variable to the mid element.

## Day 3: ##
#### [Coding Ninjas - Implement Lower Bound](https://www.codingninjas.com/codestudio/problems/lower-bound_8165382?utm_source=youtube&utm_medium=affiliate&utm_campaign=codestudio_Striver_BinarySeries) ####
   Question: You are given an array 'arr' sorted in a non-decreasing order and a number 'x'. You must return the index of the lower bound.
   - Topic: *Binary Search*
   - Difficulty: *Easy*
   - Approach: Start by writing the binary search code. Next, instead of seraching for the element in the loop, seach for a number greater than or equal to the target value. If found replace the result variable with the index of this element and the low variable to the mid-1 value; else change low to mid+1.

#### [Coding Ninjas - Implement Upper Bound](https://www.codingninjas.com/codestudio/problems/implement-upper-bound_8165383?utm_source=youtube&utm_medium=affiliate&utm_campaign=codestudio_Striver_BinarySeries) ####
   Question: You are given an array 'arr' sorted in a non-decreasing order and a number 'x'. You must return the index of the upper bound.
   - Topic: *Binary Search*
   - Difficulty: *Easy*
   - Approach: Start by writing the binary search code. Next, instead of seraching for the element in the loop, seach for a number greater than the target value. If found replace the result variable with the index of this element and the high variable to the mid-1 value; else change low to mid+1.

#### [Coding Ninjas - Ceil the Floor](https://www.codingninjas.com/studio/problems/ceiling-in-a-sorted-array_1825401) ####
   Question: You’re given an sorted array arr of n integers and an integer x. Find the floor and ceiling of x in arr\[0..n-1]. The floor of x is the largest element in the array which is smaller than or equal to x. The ceiling of x is the smallest element in the array greater than or equal to x.
   - Topic: *Binary Search*
   - Difficulty: *Medium*
   - Approach: Start by sorting the array for Binary Search. Next, call the functions for lower bound and upper bound for ceil and floor respectively. Return by making a pair of the floor and ceil values with the help of the function 'make_pair(int, int);'.

## Day 4: ##
  #### [Leetcode 34 - Find First and Last Position of Element in Sorted Array](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/) ####
  Question: Given an array of integers nums sorted in non-decreasing order, find the starting and ending position of a given target value. If target is not found in the array, return {-1, -1}.
  - Topic: *Binary Search*
  - Difficulty: *Medium*
  - Approach: Write two functions. One for the left bound(lower bound) in which when target is found the index is stored in a variable and then the value is of high becomes mid-1 and then returns the value of the lowest index and if index not found returns -1. Similarly, the other function is right bound(upper bound) but here instead of high changing the low changes to mid+1 to keep searching for the upper bound.

#### [Coding Ninjas - Number of Occurence](https://www.codingninjas.com/studio/problems/occurrence-of-x-in-a-sorted-array_630456) ####
   Question: You’re given an sorted array arr of n integers and an integer x. Find the number of occurences of x in the array.
   - Topic: *Binary Search*
   - Difficulty: *Medium*
   - Approach: Write the same solution as the previous question., that is the same code for the prev. question and then calculate the total occurence by the formula, 'first - last + 1' and return the count.

## Day 5: ##
  #### [Leetcode 33 - Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/) ####
  Question: There is an integer array nums sorted in ascending order (with distinct values). Prior to being passed to your function, nums is possibly rotated at an unknown pivot index k (1 <= k < nums.length) such that the resulting array is [nums[k], nums[k+1], ..., nums[n-1], nums[0], nums[1], ..., nums[k-1]] (0-indexed). For example, [0,1,2,4,5,6,7] might be rotated at pivot index 3 and become [4,5,6,7,0,1,2]. Given the array nums after the possible rotation and an integer target, return the index of target if it is in nums, or -1 if it is not in nums.
  - Topic: *Binary Search*
  - Difficulty: *Medium*
  - Approach: Perform a normal binary search for the element, but while searching for the element, locate the sorted half, as atleast one half has to be sorted. Check if target is in the range of the sorted half, if not eleminate the sorted half and change the values of high and low respectively.

#### [Leetcode 81 - Search in Rotated Sorted Array II](https://leetcode.com/problems/search-in-rotated-sorted-array-ii/) ####
  Question: There is an integer array nums sorted in non-decreasing order (not necessarily with distinct values). Before being passed to your function, nums is rotated at an unknown pivot index k (0 <= k < nums.length) such that the resulting array is [nums[k], nums[k+1], ..., nums[n-1], nums[0], nums[1], ..., nums[k-1]] (0-indexed). For example, [0,1,2,4,4,4,5,6,6,7] might be rotated at pivot index 5 and become [4,5,6,6,7,0,1,2,4,4]. Given the array nums after the rotation and an integer target, return true if target is in nums, or false if it is not in nums.
  - Topic: *Binary Search*
  - Difficulty: *Medium*
  - Approach: Perform a normal binary search for the element, but while searching for the element, check if the elements at mid high and low all three are equl if they are then reduce the array by eliminatnig the high and the low elements then continue to locate the sorted half, as atleast one half has to be sorted. Check if target is in the range of the sorted half, if not eleminate the sorted half and change the values of high and low respectively.

## Day 6: ##
  #### [Leetcode 153 - Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/) ####
  Question: Suppose an array of length n sorted in ascending order is rotated between 1 and n times. For example, the array nums = [0,1,2,4,5,6,7] might become [4,5,6,7,0,1,2] if it was rotated 4 times. [0,1,2,4,5,6,7] if it was rotated 7 times. Notice that rotating an array [a[0], a[1], a[2], ..., a[n-1]] 1 time results in the array [a[n-1], a[0], a[1], a[2], ..., a[n-2]]. Given the sorted rotated array nums of unique elements, return the minimum element of this array.
  - Topic: *Binary Search*
  - Difficulty: *Medium*
  - Approach: In a normal binary search, initialise a ans variable with 'INT_MAX'. In the while loop, check if element at low is less or equal to the element at high, if true then replaec ans with the minimum of low and ans. then check if low less than equal to mid, if true ans is the minimum between the mid and the low and low is mid+1 as the sorted half is now element. Now for the else case, decrease the high to mid-1 and ans is the minimum between the mid and ans.

#### [Coding Ninjas - Find out how many times the array has been rotated](https://www.codingninjas.com/studio/problems/rotation_7449070) ####
   Question: Given an integer array arr of size N, sorted in ascending order (with distinct values). Now the array is rotated between 1 to N times which is unknown. Find how many times the array has been rotated.
   - Topic: *Binary Search*
   - Difficulty: *Easy*
   - Approach: Look for the minimum number in the array and return its index.

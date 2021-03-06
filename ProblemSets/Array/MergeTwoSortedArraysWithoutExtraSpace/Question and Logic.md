# Merge Two Sorted Arrays Without Extra Space

Given two sorted arrays **arr1[]** of size **N** and **arr2[]** of size **M**. Each array is sorted in non-decreasing order. Merge the two arrays into one sorted array in non-decreasing order without using any extra space.

### Example :

```
Input:
	N = 4, M = 5
	arr1[] = {1, 3, 5, 7}
	arr2[] = {0, 2, 6, 8, 9}
	
Output: 0 1 2 3 5 6 7 8 9
```
**Explanation :** Since you can't use any extra space, modify the given arrays to form arr1[] = {0, 1, 2, 3} and arr2[] = {5, 6, 7, 8, 9}.

### Logic :

1. #### Compare and swap method :
    - Take input as two sorted arrays and there sizes a[ ], b[ ], n ( length of a ), m ( length of b).
    - take two varible `k = n-1` and `j = 0`.
    - run a while loop from `k = n-1` to `k = 0` and `j = 0` to `j = m-1`.
    - check if `a[i] > b[j]`. If yes swap them . If no `k--` and `j++`.
    - after the while loop sort both the array and print them.
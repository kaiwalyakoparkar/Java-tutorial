# Count Pairs With Given Sum

Given an array of **N** integers, and an integer **K**, find the number of pairs of elements in the array whose sum is equal to **K**.

### Example :

```
Input:
	N = 4, K = 6
	arr[] = {1, 5, 7, 1}
	
Output: 2
```
**Explanation :**
	`arr[0] + arr[1] = 1 + 5 = 6` 
	and `arr[1] + arr[3] = 5 + 1 = 6`.

### Logic :

1. #### Naive approach  :
    - Take input as an array
    - run a nested loop `i = 0` to `arr.length-2` and `j = i+1` to `arr.length-1`.
    - if `arr[i] + arr[j] == k` ( required sum ) then increment the counter

2. #### Optimized approach : 
    - Take a look at the below image and the comments in the code to understand the intution behind the algorithm ( On Notion ).

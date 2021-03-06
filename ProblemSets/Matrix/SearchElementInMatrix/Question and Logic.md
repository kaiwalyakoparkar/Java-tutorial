# Search Element In Matrix

Write an efficient algorithm that searches for a value in an **m x n** matrix. This matrix has the following properties:

- Integers in each row are sorted from left to right.
- The first integer of each row is greater than the last integer of the previous row.

### Example :

```
Input : matrix = [[1,3,5,7],[10,11,16,20],[23,30,34,60]], target = 3

Output : true
```

### Logic :

1. #### Naive Approach :
    - Take a input as an 2D array, and target (element to be found)
    - traverse the matrix in the same manner as you take the input in the matrix
    - and while traversing compare target with every element
    - if the element is found print true
    - else print false

1. #### Better Approach :
    - Take a input as an 2D array, and target (element to be found)
    - put a pointer i=0 and on the matrix as arr [ i ][ 0 ] location
    - increment i and check if the target = arr [ i ][ 0 ]
    - if yes then binary search from arr [ i ] [ 0 ] to the end of that row
    - in binary search if you find the target element then print true
    - else keep on incrementing i and at last print false

1. #### Optimal Approach : 
    - put a pointers "a = 0" and "b = row -1 " on the last element of the first row
    - run a while loop " while ( a < row && b = column ) "
    - in the loop check if arr [ a ][ b ] is equal to the target, if yes then print true
    - then check if arr [ a ][ b ] > target the decrement b
    - else increment a
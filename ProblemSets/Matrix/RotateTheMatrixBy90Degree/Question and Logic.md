# Rotate The Matrix By 90 Degree

Given a square matrix, turn it by 90 degrees in clockwise direction without using any extra space.

### Examples :

```
Input :
	1 2 3
	4 5 6
	7 8 9
	
Output :
	7 4 1
	8 5 2
	9 6 3
```

### Logic :

1. #### Brute-Force Approach :
    - Take input as a matrix and size of matrix as n
    - declare a new matrix ( rotMatrix )of size n x n
    - declare two variables p = n-1 and c = 0
    - traverse the input array and in the second (nested) loop of j add element at arr [ i ] [ j ] to rotMatrix[c++][ p ]
    - after comming out of j loop while entering again in i loop that means while changing the row in the matrix make c = 0 and p - -
    - At the end print the rotMatrix

1. #### Optimal Approach :
    - Take input as a matrix and size of matrix as n
    - make the transpose of the matris that means swap the element in the row with  element in the column
    - eg : arr[ i ] [ j ] with arr[ j ] [ i ]
    - but while doing this don't traverse the matrix as usual or else this will re-swap the previously swapped element
    - to overcome this make j = i instead of j = 0 in the second (nested ) loop
    - after this reverse the matrix row wise
    - at the end print the arr
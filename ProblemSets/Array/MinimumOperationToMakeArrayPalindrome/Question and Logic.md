# Minimum Operation To Make Array Palindrome

Given a Integer array **A[]** of **n** elements. Your task is to complete the function PalinArray. Which will return number of operation to make array palindromic.

### Example :
```
Input : 
	5
	111 222 333 111 222

Output : 1
```

### Logic :

1. #### Search and swap  :
    - Take a input as an array ans size of the array ( n ) .
    - put two pointer on first ( i ) and the last ( j ) element of the array.
    - if both are equal increase first pointer and decrease second pointer.
    - if not then run a third loop ( k ) from j-1 to ( n /2)+1 and if you find arr [ k ] equal to arr [ i ] then swap arr [ j ] and arr [ k ] and increse the counter of operation by 1 .

1. #### Using Hash Maps : 
    - Take a input as an array and size of the array ( n ) .
    - declare an Hash Map ( mp ) .
    - run a loop from ( n/2) to n-1 and add all the " elements and their locations " in the map ( mp ) .
    - then keep two pointers ( i ) on first location of the array and ( j ) of the last location of the array respectively.
    - compare if arr[ i ] is equal to arr[ j ] if yes then increment i and decrement j .
    - if no then check if arr[ i ] is present in the map if yes then get the value of arr[ i ] in k and swap arr [ k ] and arr [ j ] .
    - continue this process till i = j .
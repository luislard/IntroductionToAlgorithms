## 2.1-3 Search Problem

Consider the searching problem: 

Input: A sequence of n numbers A = [a1..an]  and a value "v". 

Output: An index i such that v = A[i] or the special value NIL if "v" does not appear in A. 

Write pseudocode for linear search, which scans through the sequence, looking for "v". Using a loop invariant, prove that your algorithm is correct. Make sure that your loop invariant fulfills the three necessary properties.


```
// we start stating the value is not found
i = NIL

// for the sake of my brain arrays starts at 0 not 1!
for j = 0 to j < A.length and i !== NIL
    if A[j] == v
        i = j
```

Our loop invariant is the i value itself

Initialization:
Prior first iteration i = NIL.

Maintenance:
After our first iteration if the value is found the value is not NIL and the loop stops
Otherwise, the loops continues

Termination:
The algoritm ends when the loop reaches the length of the array, if a value was found we would have i !== NIL otherwise i === NIL since we never assigned a different value.
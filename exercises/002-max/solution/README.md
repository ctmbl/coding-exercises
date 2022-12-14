## Solution

The trick is to only remember the maximum found and test each element of `L` against it.  
However the difficulty is too properly defined the initial state of the max.  
If we set it to 0, computing the max of a list full of negative numbers would fail.  
We must set it to the first value of `L` and then update it once we found a greater element.

*Solution:*
```py
def max_list(L):
    ret = L[0]
    for i in L:
        if i > ret:
            i = ret
    return ret
```

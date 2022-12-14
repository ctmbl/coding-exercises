## Solution

You have to simply sum every element (that should be numbers) of L and divide by the number of element.
The sum is easily computed with a `for` loop, and `len` gives you the number of element.

*Solution:*
```py
def average(L):
    S = 0
    for i in L:
        S += i
    return S / len(L)
```

#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) 
```python
         a = 0
        while (a < n * n * n):
        a = a + n * n
```
## Runtime complexity is O(n), and the runtime is proportionate to size of n





b) 
```python sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2 sum += 1
```
## Runtime complexity is `O(n)`. The larger `n` gets, the more time the code will take to run on a linear scale.






c)  
```python def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```
## Runtime complexity is `O(1)`. The function only checks if bunnies exists. The number of bunnies does not change the runtime duration.








## Exercise II

This pseudocode has an O(log n) runtime.

1. Drop the egg from middle floor. 

        If the return value is "Egg Broke", 
            move to the current floor minus one 
            try again until return is "Egg Not Broke"

2.      If the return value from the middle floor is "Egg Not Broke", 
            move to the current floor plus one 
            until the return value is "Egg Broke"

3.      Once the return value is "Egg Broke" 
            move to the current floor minus one
            return.



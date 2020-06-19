# Analysis of Algorithms

## Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```python
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```
n = 3
a less than 3*3*3 27
0 + 9
9 + 9
18 + 9

a less than 4*4*4 =64
0 + 16
16 + 16
32 + 16
48 + 16
time

```
b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
```

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```

bunnies = 5
returns 2+bunnyEars(4)
    returns 2+bunnyEars(3)
      returns 2+bunnyEars(2)
        returns 2+bunnyEars(1)
          returns 2+bunnyEars(0)
returns 0



## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.

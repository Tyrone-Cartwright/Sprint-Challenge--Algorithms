Add your answers to the Algorithms exercises here.

## Exercise I

```
a)  a = 0
    while (a < n * n * n):
      a = a + n * n

O(n) it grows by n. So whatever n is equal to the while loop will run that many times, ex: if n = 2 the while loop runs twice, if n = 4 then the while loop will run four times.
```

```
b)  sum = 0 --> O(n)

    for i in range(n): --> O(n)
      i += 1

      for j in range(i + 1, n): --> O(n)
        j += 1

        for k in range(j + 1, n): --> O(n)
          k += 1

          for l in range(k + 1, 10 + k): --> O(1)
            l += 1

            sum += 1

This will be O(n^3) because there are four nested loops within this function.
```

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)

This will be O(n) as the calculations will equal the length of the input
```

## Exercise II

I would use a Binary Search algorithm, I would start at the middle floor and drop an egg. If it breaks, we can conclude that f must be on the lower half of the building. So then we move to the middle of the building and drop another egg. Then we can cut the remaining possible floors in half and drop another egg, and see if the middle value is too high or too low. In this way we will arrive at floor f in O(log(n)) steps.

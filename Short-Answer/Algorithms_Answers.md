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

          for l in range(k + 1, 10 + k): --> O(n)
            l += 1

            sum += 1

This will be O(n^4) because there are four nested loops within this function.
```

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)

This will be O(n) as the calculations will equal the length of the input
```

# SWE_2021_41_2024_2_week_6

___

## Week 4 Assignment
* [Repository](https://github.com/NHJin99/SWE_2021_41_2024_2_week_4)

```c
def isHappy(n):

  nset = set()
  nset.add(n)


  while n!=1:
    sum = 0
    while n!=0:
      a = n - 10*(n//10)
      n = n//10
      sum += a*a

    n = sum
    if n in nset:
      print("False")
      return
    nset.add(n)

  print("True")
  return
```

* An algorithm to determine if a number n is happy.
* A happy number is a number defined by the following process:

  * Starting with any positive integer, replace the number by the sum of the squares of its digits.
  * Repeat the process until the number equals 1 (where it will stay), or it loops endlessly in a cycle which does not include 1.
  * Those numbers for which this process ends in 1 are happy.

* Return true if n is a happy number, and false if not.

___

## Week 5 Assignment
> doker 

# SWE_2021_41_2024_2_week_6

___

## Week 4 Assignment
* [repository](https://github.com/NHJin99/SWE_2021_41_2024_2_week_4)

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

* Description of my code

___

## Week 5 Assignment
> doker 

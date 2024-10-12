# SWE_2021_41_2024_2_week_6

___

## Week 4 Assignment
* __[Repository](https://github.com/NHJin99/SWE_2021_41_2024_2_week_4)__

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

* An algorithm to determine if a number __n__ is happy.
* A __happy number__ is a number defined by the following process:

  * Starting with any positive integer, replace the number by the sum of the squares of its digits.
  * Repeat the process until the number equals 1 (where it will stay), or it __loops endlessly in a cycle__ which does not include 1.
  * Those numbers for which this process __ends in 1__ are happy.

* Return __true__ if n is a happy number, and __false__ if not.
* Constraints: $1 \leq n \leq 2^{31}-1$

___

## Week 5 Assignment
> ```shell
> docker exec ossp-container cat /etc/os-release
> ```
> * This conmmand checks container's OS
> 
>   ![LinuxOs](https://github.com/user-attachments/assets/80ab6e5d-1afe-4c46-b3b6-09cab93b7517)


> ```shell
> docker exec ossp-container git --version
> ```
> * This conmmand checks container's git version
>
>    ![Git](https://github.com/user-attachments/assets/f76a07aa-4771-4559-9142-0f7d5b6f4ae8)


> ```shell
> docker exec ossp-container python3 --version
> ```
> * This conmmand checks container's python3 version
>
>    ![Python3](https://github.com/user-attachments/assets/2bf74d47-053c-4015-bfe5-50126da819f4)


> ```shell
> docker inspect --format="{{ .HostConfig.Binds }}" ossp-container
> ```
> * This conmmand checks container's path of mounted directory
> * The format is as following: __‘[<host_dir_path>:<container_dir_path>]’__
>
>    ![Bindmount](https://github.com/user-attachments/assets/1596a180-f64c-41d4-817a-ab6fe1433f3c)



# SWE_2021_41_2024_2_week_6

---

## Week 4 Assignment

* https://github.com/kimhanbalk/SWE_2021_41_2024_2_week_4

```python
def isHappy(n):
  repeat = set()
  while n!=1:
    if n in repeat:
      return False
    repeat.add(n)
    digits = [int(digit) for digit in str(n)]
    squared_sum = sum([x**2 for x in digits])
    n= squared_sum
  return True
```

* This code is designed to find happy number. A happy number is defined as a number where, when the sum of the squares of its digits is repeatedly calculated, the final result eventually becomes 1. I will explain the algorithm of this code.
\
First, a set() called repeat is created to prevent duplicates. The digits of the given number are extracted and the sum of their squares is calculated. If summed value becomes 1, the function returns true and exits loop. If the value is not 1, it checks if the value exists in the repeat set. If it has already been calculated before, it indicates an infinite loop, so the function returns false and exits loop. If the value has not been calculated yet, it is added to the repeat set and continues the loop again.

---

## Week 5 Assignment
> ```bash
> docker exec ossp cat /etc/os-release
> ```
> * This code is used to output the operating system information within the Docker container named 'ossp'.

> ```bash
> docker exec ossp git --version
> ```
> * This code retrieves the version of Git installed the Docker container 'ossp'.

> ```bash
> docker exec ossp python3 --version
> ```
> * This code retrieves the version of Python installed the Docker container 'ossp'.

> ```bash
> docker inspect --format"{{ .HostConfig.Binds }}" ossp
> ```
> * This code displays bind mounts configured for the Docker container 'ossp'.

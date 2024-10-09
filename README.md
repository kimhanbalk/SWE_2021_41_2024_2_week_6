# SWE_2021_41_2024_2_week_6
## Week 4 Assignment

__unordered list___(*,-)

*https://github.com/kimhanbalk/SWE_2021_41_2024_2_week_4

'''python
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
'''

-This code is designed to find happy number that satiesfies a specific mathematical rule. A happy number is defined as a number where, when the sum of the squares of its digits is repeatedly calculated, the final result eventually becomes 1.

## Week 5 Assignment

> docker exec ossp cat /etc/os-release
>> explanation

> docker exec ossp git --version
>> explanation

> docker exec ossp python3 --version
>> explanation

> docker inspect --format"{{ .HostConfig.Binds }}" ossp
>> explanation

# SWE_2021_41_2024_2_week_6
## Week 4 Assignment
###### https://github.com/soo030/SWE_2021_41_2024_2_week_4.git
```python
def isHappy(n):
  change = set()

  while n!= 1 and n not in change:

    change.add(n)
    calculate = 0

    while n > 0:
      tmp = n % 10
      n = n // 10
      calculate += tmp ** 2

    n = calculate

  return n == 1
```
* 

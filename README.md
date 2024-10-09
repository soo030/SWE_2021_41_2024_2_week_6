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
* Explanation of the code
1. make set 'change' which contains records of sum of the squares of the number's digits
2. add current number 'n' to 'change'
3. calculate sum of the squares of the number's digits and save it to 'n'
4. go to step 2 and repeat while 'n' is not 1 or 'n' is not in 'change'
5. if n is 1, return True (happy number)
6. if not, return False
___
## Week 5 Assignment
> ```bash
> docker exec ossp-container cat /etc/os-release
> ```
> * Explanation
> * output

> ```bash
> docker exec ossp-container git --version
> ```
> *
> * output

> ```bash
> docker exec ossp-container python3 --version
> ```
> *
> * output

> ```bash
> docker inspect --format="{{ .HostConfig.Binds }}" ossp-container
> ```
> *
> * output

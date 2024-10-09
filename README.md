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
> * runs container and checks version/
> __Output__
> ```bash
> PRETTY_NAME="Ubuntu 24.04.1 LTS"
> NAME="Ubuntu"
> VERSION_ID="24.04"
> VERSION="24.04.1 LTS (Noble Numbat)"
> VERSION_CODENAME=noble
> ID=ubuntu
> ID_LIKE=debian
> HOME_URL="https://www.ubuntu.com/"
> SUPPORT_URL="https://help.ubuntu.com/"
> BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
> PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
> UBUNTU_CODENAME=noble
> LOGO=ubuntu-logo
> ```

> ```bash
> docker exec ossp-container git --version
> ```
> * prints the version of git if successfully installed\
> __Output__
> ```bash
> git version 2.43.0
> ```

> ```bash
> docker exec ossp-container python3 --version
> ```
> * prints the version of python3 if successfully installed\
> __Output__
> ```bash
> Python 3.12.3
> ```

> ```bash
> docker inspect --format="{{ .HostConfig.Binds }}" ossp-container
> ```
> * prints path of mounted directory of the specified container\
> __Output__
> ```bash
> [/root/ossp_host_dir:/mnt/ossp_container_dir]
> ```

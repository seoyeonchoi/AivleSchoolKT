## 추가 실습 Q3 답안
#문제 링크# -> https://www.acmicpc.net/problem/1110
#답안 코드#

```python
def add_N(N):
    count = 1
    first = N
    while(True):    
        ten = (N%10)*10
        one = (N//10 + N%10)%10
        N = ten + one
        if N == first:
            break
        else:
            count += 1

    return count

print(add_N(N))
```

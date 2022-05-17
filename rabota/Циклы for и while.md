7.1 Цикл for
2/10 шаг:
for i in range(10):
    print("Python is awesome!")
3/10 шаг:
a = input()
b = int(input())
for i in range(b):
    print(a)
4/10 шаг:
for i in range(6):
    print('A' * 3)
for i in range(5):
    print('B' * 4)
print('E')
for i in range(9):
    print('T' * 5)
print('G')
5/10 шаг:
n = int(input())
for i in range(n):
    print('*' * 19)
7/10 шаг:
a = input()
for b in range(10):
    print(b, a)
8/10 шаг:
n=int(input())
for i in range(n+1):
    print('Квадрат числа', i, 'равен', i**2)
9/10 шаг:
n = int(input())
for i in range(n):
    print('*' * (n - i))
10/10 шаг:
m=int(input())
p=int(input())
n=int(input())
for i in range(n):
    print(i+1,m)
    m=m+m*p/100
    ![image](https://user-images.githubusercontent.com/97594452/168923848-18bf9ed5-094b-4209-af74-dcbf6421918d.png)

7.2 Цикл for: функция range
7/11 шаг:
c = int(input())
v = int(input())
for i in range (c, v+1):
    print(i)
8/11 шаг:
n, m = int(input()), int(input())

if n < m:
    for i in range(n, m + 1):
        print(i)
else:
    for i in range(n, m - 1, -1):
        print(i)
9/11 шаг:
m, n = int(input()), int(input())
for i in range(m - 1 + m % 2, n - 1, -2):
    print(i)
10/11 шаг:
m, n = int(input()), int(input())
for i in range(m, n + 1):
    if i % 17 == 0 or i % 10 == 9 or i % 15 == 0:
        print(i)
11/11 шаг:
a = int(input())

for i in range(1, 11):
    print(f"{a} x {i} = {i*a}")
    ![image](https://user-images.githubusercontent.com/97594452/168925519-00c68b43-790c-4755-88f3-8ca8a25b306f.png)

7.3 Частые сценарии
5/16 шаг:
a = int(input())
b = int(input())
count = 0
for i in range(a, b + 1):
    if i % 10 == 4 or i % 10 == 9:
        count += 1
print(count)
6/16 шаг:
a = int(input())
s = 0
for i in range(a):
    s += int(input())
print(s)
7/16 шаг:
n=int(input())
from math import *
s=0
for i in range(n):
    s+=(1/(i+1))
print(s-log(n))
8/16 шаг:
n = int(input())
total=0
for i in range(n+1):
    if i%10==5:
        total+=i
print(total)
9/16 шаг:
n = int(input())
total = 1
for i in range(1, n + 1):
    total *= i
print(total)
10/16 шаг:
p = 1
for _ in range(10):
    n = int(input())
    p *= n + (n == 0)
print(p)
11/16 шаг:
n, s = int(input()), 0
for i in range(1, n + 1):
    if n % i == 0:
        s += i
print(s)
12/16 шаг:
n = int(input())

if (n % 2 == 0):
    print(-n // 2)
else:
    print(n // 2 + 1)
13/16 шаг:
n = int(input())

max1, max2 = -1, -1

for _ in range(n):
    num = int(input())
    if num > max1:
        max2 = max1
        max1 = num
    elif num > max2:
        max2 = num
        
print(max1)
print(max2)
14/16 шаг:
f = 'YES'
for _ in range(10):
    if int(input())%2:
        f = 'NO'
print(f)
15/16 шаг:
n = int(input())
a, b = 1, 1

for i in range(n):
    print(a, end=' ')
    a, b = b, a + b
![image](https://user-images.githubusercontent.com/97594452/168926935-962906c3-c182-4707-a800-ac4b63704529.png)

7.4 Цикл while
8/14 шаг:
a = input()
while (a!='КОНЕЦ'):
    print(a)
    a = input()
9/14 шаг:
a = input()
while a != 'КОНЕЦ' and a != 'конец':
    print(a)
    a = input()
10/14 шаг:
a, k = input(), 0
while a not in ('стоп', 'хватит', 'достаточно'):
    k += 1
    a = input()
print(k)
11/14 шаг:
n = int(input())
while n % 7 == 0:
    print(n)
    n = int(input())
12/14 шаг:
a = int(input())
b = 0
while a >= 0:
    b += a
    a = int(input())
print(b)
13/14 шаг:
n, k = int(input()), 0
while 1 <= n <= 5:
    k += n == 5
    n = int(input())
print(k)
14/14 шаг:
n = int(input())
k = 0
for i in (25, 10, 5, 1):
    while n // i > 0:
        k += 1
        n -= i
print(k)
![image](https://user-images.githubusercontent.com/97594452/168927975-83846327-3061-40e5-903f-2941e5cdf2d0.png)

7.5 Цикл while: обработка цифр числа
4/10 шаг:
n = int(input())
while n:
    print(n % 10)
    n //= 10
5/10 шаг:
n = int(input())
while n != 0:
    print(n % 10, end = '')
    n = n // 10
6/10 шаг:
a =input()
print("Максимальная цифра равна", max(a))
print("Минимальная цифра равна", min(a))
7/10 шаг:
n,sm,kol,pr = int(input()),0,0,1
np = n % 10
while n != 0:
    sm += n % 10 
    kol +=1
    pr *= n % 10
    n1 = n
    n = n // 10
print(sm,kol,pr,sm/kol,n1,n1+np,sep='\n')
8/10 шаг:
n = int(input())
while n > 99:
    n //= 10
print(n % 10)
9/10 шаг:
n = int(input())
m = n % 10
answer = 'YES'
while n != 0:
    if m != n % 10:
        answer = 'NO'
    n = n // 10
print(answer)
10/10 шаг:
n,b = int(input()),'YES'
while n // 10 != 0 :
    a = n % 10  
    n = n // 10
    if a > n % 10:
        b = 'NO'
print(b)
![image](https://user-images.githubusercontent.com/97594452/168928678-5852d36f-7d20-4d47-876b-4c9155fe982c.png)

7.6 break, continue и else
7/12 шаг:
n, div = int(input()), 2
while n % div:
    div += 1
print(div)
8/12 шаг:
n = int(input())
for i in range(1, n + 1):
    if 5 <= i <= 9 or 17 <= i <= 37 or 78 <= i <= 87:
        continue
    print(i)
![image](https://user-images.githubusercontent.com/97594452/168928893-ad1dd6c3-551a-4fc5-ae3d-3ebbf9375b53.png)

7.7 Поиск ошибок и ревью кода
3/8 шаг:
count = 0
p = 1
for i in range(1, 11):
    x = int(input())
    if x >= 0:
        p = p * x
        count = count + 1
if count > 0:
    print(count)
    print(p)
else:
    print('NO')
4/8 шаг:
mx = -10**6 - 1
s = 0
for i in range(10):
    x = int(input())
    if x < 0:
        s += x
    if x < 0 and x > mx:
        mx = x
if s < 0:
    print(s)
    print(mx)
else:
    print('NO')
5/8 шаг:
s = 0
for _ in range(7):
    n = int(input())
    if n % 2 == 0:
        s += n
print(s)
6/8 шаг:
n = int(input())
max_digit = -1
while n > 0:
    digit = n % 10
    if digit % 3 == 0:
        if digit > max_digit:
            max_digit = digit
    n = n // 10
if max_digit == -1:
    print('NO')
else:
    print(max_digit)
7/8 шаг:
n = int(input())
while n > 9: 
    n //= 10
print(n)
8/8 шаг:
n = int(input())
product = 1
while n > 0:
    digit = n % 10
    product *= digit
    n //= 10
print(product)
![image](https://user-images.githubusercontent.com/97594452/168929313-c19ff417-ecf6-4006-aec6-838fe8f29150.png)

7.8 Вложенные циклы. Часть 1
5/13 шаг:
n = int(input())
for i in range(n):
    print(n, n, n)
6/13 шаг:
n = int(input())
for i in range(1, n + 1):
    for _ in range(5):
        print(i,"", end='')
    print()
7/13 шаг:
n = int(input())
for i in range(1, n + 1):
    for  j in range(1, 10):
        print(i,'+', j, '=', i + j)
    print()
8/13 шаг:
n = int(input())
for i in range(1, n + 1):
    print('*' * min(i, n - i + 1))
9/13 шаг:
for i in range(1, int(input()) + 1):
    print(str(i) * i)
![image](https://user-images.githubusercontent.com/97594452/168929692-de8d84ea-8cc6-48ff-8dc6-34ad1e04f035.png)

7.9 Вложенные циклы. Часть 2
1/7 шаг:
p =0
n = int(input())
for i in range(n):
    for j in range(i + 1):
        print(p+1, end=' ')
        p+=1
    print()
2/7 шаг:
n = int(input())
for i in range(1, n + 1):
    for j in range(1, 2 * i):
        print(min(j, 2 * i - j), end='')
    print()
3/7 шаг:
a , b = int(input()), int(input())
total_maximum = 0
digit = 0

for i in range(a, b + 1):
    maximum = 0
    for j in range(1, i + 1):
        if i % j == 0:
            maximum += j
        if maximum >= total_maximum:
            total_maximum = maximum
            digit = j
print(digit, total_maximum)
4/7 шаг:
n = int(input())
for i in range(1, n+1):
    print(i, end = '')
    for j in range(1, i+1):
        if i%j == 0:
            print('+', end = '')
    print()
5/7 шаг:
n = int(input())
while n // 10 > 0:
    n = n // 10 + n % 10
print(n)
6/7 шаг:
n = int(input())
a = 1
b = 0
for i in range(1, n + 1):
    a *= i
    b += a
print(b)
7/7 шаг:
a, b, = int(input()), int(input())
for i in range(a, b + 1):
    if i == 1:
        continue
    for j in range(2, i):
        if i % j == 0:
            break
    else:
        print(i)
![image](https://user-images.githubusercontent.com/97594452/168929903-570b249a-2c41-4dd3-ad3d-1d7f5e7dd820.png)












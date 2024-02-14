```python
a = int(input())
b = int(input())
c = int(input())
d = int(input())
a = 1
b = 2
c = 3
d = 4
ab = 0
cd = 0
c = int(input())

if (b - a) == (c - b):
    print("YES")
else:
    print("NO")
if a > b:
    ab = b
    print(a)
if c > d:
    cd = d
    print(c)
if ab > cd:
    print(cd)
else:
    print(ab)

a = int(input())
b = int(input())
c = int(input())
d = int(input())
if a > b:
    a = b
if c > d:
    c = d
if a > c:
    print(c)
else:
    print(a)

num = int(input())
if num <= 13:
    print("детство")
if 14 <= num <= 24:
    print("молодость")
if 25 <= num <= 59:
    print("зрелость")
if num >= 60:
    print("старость")

a = int(input())
b = int(input())
c = int(input())

if a > 0:
    a = a
else:
    a = 0
if b > 0:
    b = b
else:
    b = 0
if c > 0:
    c = c
else:
    c = 0

print(a+b+c)

a = 2
b = 4
c = 6
if not (c <= 10):
    print("true")
else:
    print("false")

a = int(input())

if a > -30 and a <= -2 or a > 7 and a <= 25:
    print("Принадлежит")
else:
    print("Не принадлежит")

a= int(input())

if 999 < a < 10000 and (a % 7 == 0 or a % 17 == 0):
    print("YES")
else:
    print("NO")



a, b, c = int(input()), int(input()), int(input())

if a == b:
    if b == c:
        print(3)
    else:
        print(2)
else:
    if a == c:
        print(2)
    else:
        if b == c:
            print(2)
        else:
            print(0)


a, b, c = int(input()), int(input()), int(input())

if a == b == c:
    print(3)
elif a == b:
    print(2)
elif b == c:
    print(2)
elif a == c:
    print(2)
else:
    print(0)


a, b, c = int(input()), int(input()), int(input())

if a == b == c:
    print(3)
elif a == b or b == c or a == c:
    print(2)
else:
    print(0)

a = int(input())
b = int(input())
c = int(input())

if a == b == c:
    print("Равносторонний")
elif a == b or a == c or b == c:
    print("Равнобедренный")
else:
    print("Разносторонний")

color1 = input()
color2 = input()

if (color1 == "красный" or color2 == "красный") and (color2 == "синий" or color1 == "синий"):
    print("фиолетовый")
elif (color1 == "красный" or color2 == "красный") and (color2 == "желтый" or color1 == "желтый"):
    print("оранжевый")
elif (color1 == "синий" or color2 == "синий") and (color2 == "желтый" or color1 == "желтый"):
    print("зеленый")
elif color1 == color2 and (color1 == "красный" or color1 == "синий" or color1 == "желтый"):
    print(color1)
else:
    print("ошибка цвета")

if x == 0:
    print("зеленый")
elif 1 <= x <=10:
    if x % 2 == 0:
        print('черный')
    else:
        print("красный")
elif 11 <= x <= 18:
    if x % 2 != 0:
        print('черный')
    else:
        print("красный")
elif 19 <= x <= 28:
    if x % 2 == 0:
        print('черный')
    else:
        print("красный")
elif 29 <= x <= 36:
    if x % 2 != 0:
        print('черный')
    else:
        print("красный")
else:
    print("ошибка ввода")

x1, y1, x2, y2 = int(input()), int(input()), int(input()), int(input())

if (x1 + x2 + y1 + y2) % 2 ==0:
    print("YES")
else:
    print("NO")

x = int(input())

x1 = x // 100
x2 = x // 10 % 10
x3 = x % 10
minimum = min(x1, x2, x3)
maximum = max(x1, x2, x3)

if maximum - minimum == x1 + x2 + x3 - minimum - maximum:
    print("Число интересное")
else:
    print("Число неинтересное")

c1 = len(input())
c2 = len(input())
c3 = len(input())

len_max = max(c1, c2, c3)
len_min = min(c1, c2, c3)
# поиск среднего
len_sred = c1 + c2 +c3 - len_max - len_min

if len_sred - len_min == len_max -  len_sred:
    print("YES")
else:
    print("NO")

c1 = input()

if "@" in c1 and "." in c1:
    print("YES")
else:
    print("NO")

import math

num1 = math.sqrt(2)     # вычисление квадратного корня из двух
num2 = math.ceil(3.8)   # округление числа вверх
num3 = math.floor(3.8)  # округление числа вниз

print(num1)
print(num2)
print(num3)

from math import *

num1 = sqrt(2)     # вычисление корня квадратного из двух
num2 = ceil(3.8)   # округление числа вверх
num3 = floor(3.8)  # округление числа вниз

print(num1)
print(num2)
print(num3)

from math import sqrt, ceil

print(sqrt(25))
print(ceil(34.7))

print(floor(12.8))  # приведет к ошибке, так как функция floor не подключена

# x_pow = pow(x1 - x2, 2)
# y_pow = pow(y1 - y2, 2)
print(sqrt(pow(x1 - x2, 2) + pow(y1 - y2, 2)))
# xy_sqrt = sqrt(x_pow + y_pow)
#
# print(xy_sqrt)
```
#print("Hello world")

"""a = 3
print(type(a))
a = 3.5
print(type(a))
a = "qwerty"
print(type(a))
a = "123"
print(type(a))
#Указывает тип данных a
a = a + 1
print(type(a))"""

"""a = int(5.7)
print(a)
b = int(-5.7)
print(b)
c = int(float(3**39))
d = int(3**39)
x = c-d
print(x)"""

"""name = input("Ваше имя: ")
print("Привет"+","+name+"!")"""

"""x = int(input("Сколько часов: "))
y = int(input("Сколко минут: "))
a = ((x*60) + y)*2
print(a)"""

"""a = False
b = True
c = False
print(not (a or b)and c)"""

"""a = int(input("Введите год: "))
if (a % 4 == 0 and a % 100 != 0) or (a % 400 == 0):
    print("С днем рождения!")
elif(a<1900 or a>3000):
    print("Год не входит в выборку!")
else:
    print("Год обычный!")"""

"""i = 1
while i <= 20:
    if i % 2 == 0:
        print(i)
    i += 1"""

"""i = 1
sum = 0
while i:
    i = int(input())
    sum += i
print(sum)"""

"""i = 1
x = int(input())
y = int(input())
while i:"""

"""for i in range (0,20):
    if (i % 2 == 0):
        print(i)"""

"""a, b, c, d = [int(input()) for i in range(4)]
print('', end='\t')
for j in range(c, d + 1):
    print(j, end='\t')
print()
for i in range(a, b + 1):
    print(i, end='\t')
    for j in range(c, d + 1):
        print(i * j, end='\t')
    print()"""

"""def zm(n): #создание функции
    dx, dy = 1, 0 #приращения для переменных
    x, y = 0, 0 #переменные
    arr = [[None] * n for _ in range(n)] #создание списка списков с пустыми переменными
    for i in range(1, n**2 + 1): # выполняется перебор
        arr[x][y] = i
        nx, ny = x+dx, y+dy
        if 0 <= nx < n and 0 <= ny < n and not arr[nx][ny]: #если индекс не выскочил за пределы матрицы или не наткнулся на занятую ечейку,то перменные остаются
            x, y = nx, ny
        else:
            dx, dy = -dy, dx # разворот на 90 градусов методом замены приращения,минус для чередования движения вверх и влево, а не только вправо и вниз-спираль
            x, y = x+dx, y+dy # изменнное движение для новых занчений
    for x in list(zip(*arr)):
        print(*x)

zm(int(input()))"""

"""import time
while True:
    print("Работайте!")
    time.sleep(10.0)
    print("Вы долго смотрели в монитор,теперь посмотрите в окно!")
    time.sleep(10.0)"""

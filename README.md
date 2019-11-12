# python-laboratory
import re
print( """КМ-94 Малінін Ростислав Петрович
Варіант 17 Завдання 1""")
def do_input_float(message):
    flag = True
    while flag:
        value = input(message)
        if bool(re.match('^[0-9]{1,}(\.[0-9]{1,})?$', value)):
            flag = False
            value = float(value)
        else:
            print('Помилка')
    return value
value1 =do_input_float("Введіть число\n")
value2 =do_input_float("Введіть число\n")
print(value1 & value2)
print(value1 | value2)
print(value1 ^ value2)
# "Завдання 1"
import re


def do_input_float(message):
    flag = True
    while flag:
        value = input(message)
        if bool(re.match('^[0-9]{1,}(\.[0-9]{1,})?$', value)):
            flag = False
            value = float(value)
        else:
            print('Помилка')
    return value


t1 = do_input_float("Введіть кількість балів Іванова у першому турі\n")
p1 = do_input_float("Введіть кількість балів Іванова у другому турі\n")
n1 = do_input_float("Введіть кількість балів Іванова у третьому турі\n")
print("\n")

t2 =do_input_float("Введіть кількість балів Петров у першому турі\n")
p2 =do_input_float("Введіть кількість балів Петров у другому турі\n")
n2 =do_input_float("Введіть кількість балів Петров у третьому турі\n")
print("\n")

t3 =do_input_float("Введіть кількість балів Сидоров у першому турі\n")
p3 =do_input_float("Введіть кількість балів Сидоров у другому турі\n")
n3 =do_input_float("Введіть кількість балів Сидоров у третьому турі\n")
print("\n")

value1 = t1+p1+n1
value2 = t2+p2+n2
value3 = t3+p3+n3

if value1 > value2:
    if value1 > value3:
        print("Іванов виграв!!!")
    else:
          print("Сидоров виграв!!!")
elif value1 < value2:
        if value2 > value3:
            print("Петров виграв!!!")
        else:
            print("Сидоров виграв!!!")
# "Завдання 2"
import re


def do_input_float(message):
    flag = True
    while flag:
        value = input(message)
        if bool(re.match('^[0-9]{1,}(\.[0-9]{1,})?$', value)):
            flag = False
            value = float(value)
        else:
            print('Помилка')
    return value

x = do_input_float("Введіть число \n")
if x > 3:
    x = 1.2 * x ** 2 - 3 * x - 9
    print("Значкння x =", x)
else:
    x = 12.1 / (2 * x ** 2 + 1)
    print("Значення x =", x)
# "Завдання 3"
import re


def do_input_float(message):
    flag = True
    while flag:
        value = input(message)
        if bool(re.match('^[0-9]{1,}(\.[0-9]{1,})?$', value)):
            flag = False
            value = float(value)
        else:
            print('Помилка')
    return value


def do_input_int(message):
    flag = True
    while flag:
        value = input(message)
        if bool(re.match('^[0-9]{1,}$', value)):
            flag = False
            value = int(value)
        else:
            print('Помилка')
    return value


n=do_input_int("Введіть кількість повторів\n")
x=do_input_float("Введіть значення x\n")
sum=0
for i in range(n):
    sum=sum+x/2**i
print("Значення суми",sum)
# "Завдання 4"
import re


def do_input_int(message):
    flag = True
    while flag:
        value = input(message)
        if bool(re.match('^[0-9]{1,}$', value)):
            flag = False
            value = int(value)
        else:
            print('Помилка')
    return value



N=do_input_int("Введіть межі піднесення до квадрату\n")
for i in range(N):
     if N > 0:
        if i * i <= N:
             k = i
        else:
            print("Введіть додатне число")
print("Найбільше ціле число K =",k)
# "Завдання 5"

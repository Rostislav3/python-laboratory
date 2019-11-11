# python-laboratory
value1 = int(input("Введіть число\n"))
value2 = int(input("Введіть число\n"))
print(value1 & value2)
print(value1 | value2)
print(value1 ^ value2)
# "Завдання 1"
t1 = float(input("Введіть кількість балів Іванова у першому турі\n"))
p1 = float(input("Введіть кількість балів Іванова у другому турі\n"))
n1 = float(input("Введіть кількість балів Іванова у третьому турі\n"))
print("\n")

t2 = float(input("Введіть кількість балів Петров у першому турі\n"))
p2 = float(input("Введіть кількість балів Петров у другому турі\n"))
n2 = float(input("Введіть кількість балів Петров у третьому турі\n"))
print("\n")

t3 = float(input("Введіть кількість балів Сидоров у першому турі\n"))
p3 = float(input("Введіть кількість балів Сидоров у другому турі\n"))
n3 = float(input("Введіть кількість балів Сидоров у третьому турі\n"))
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
value = float(input("Введіть число \n"))
if value > 3:
    value = 1.2 * value ** 2 - 3 * value - 9
    print("Значення x =", value)
else:
    value = 12.1 / (2 * value ** 2 + 1)
    print("Значення x =", value)
# "Завдання 3"

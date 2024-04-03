# Домашнее задание к лекции 2.«Условные конструкции. Операции сравнения»

## Задача №1

Задачи на [hackerrank](https://www.hackerrank.com/domains/python):  
Решить задачу на hackerrank ["Python If-Else"](https://www.hackerrank.com/challenges/py-if-else/problem).

## Ответ

["Python If-Else"](https://www.hackerrank.com/challenges/py-if-else/problem?isFullScreen=true)

```
if __name__ == '__main__':
    n = int(input().strip())
if n % 2 != 0:
  print("Weird")
elif n % 2 == 0 and 2 <= n <= 5:
  print("Not Weird")
elif n % 2 == 0 and 6 <= n <= 20:
  print("Weird")
elif n % 2 ==0 and n > 20:
  print("Not Weird")
```

## Задача №2

На лекции мы рассматривали пример для военкомата. Сейчас мы знаем про его рост. Расширить это приложение следующими условиями:

1. Проверка на возраст призывника.
2. Количество детей.
3. Учится ли он сейчас.

## Ответ

```
age = int(input("Введите возраст: "))
height = int(input("Введите рост: "))
children = int(input("Введите количество детей: "))
student = str(input("Учитесь ли вы сейчас (да/нет): "))
if 18 <= age <= 27:
  if children < 2:
    if student == "нет":
        if 0 <= height < 170:
          print("В танкисты")
        elif 170 <= height < 180:
          print("Во флот")
        elif 180 <= height < 200:
          print("В десантники")
        else:
          print("В другие войска")
    else:
      print("Отсрочка на время обучения")
  else:
    print("Не годен, по количеству детей")
else:
  print("Непризывной возраст")
```

## Задание №3

Разработать приложение для определения знака зодиака по дате рождения.  
Пример:

```
Введите месяц: март
Введите число: 6

Вывод:
Рыбы
```

```
month = int(input("Введите месяц рождения: "))
number = int(input("Введите число рождения: "))
if (month == 1 and number >= 21) or (month == 2 and number <= 19):
  print("Водолей")
if (month == 2 and number >= 20) or (month == 3 and number <= 20):
  print("Рыбы")
if (month == 3 and number >= 21) or (month == 4 and number <= 20):
  print("Овен")
if (month == 4 and number >= 21) or (month == 5 and number <= 21):
  print("Телец")
if (month == 5 and number >= 22) or (month == 6 and number <= 21):
  print("Близнецы")
if (month == 6 and number >= 22) or (month == 7 and number <= 22):
  print("Рак")
if (month == 7 and number >= 23) or (month == 8 and number <= 21):
  print("Лев")
if (month == 8 and number >= 22) or (month == 9 and number <= 23):
  print("Дева")
if (month == 9 and number >= 24) or (month == 10 and number <= 23):
  print("Весы")
if (month == 10 and number >= 24) or (month == 11 and number <= 22):
  print("Скорпион")
if (month == 11 and number >= 23) or (month == 12 and number <= 22):
  print("Стрелец")
if (month == 12 and number >= 23) or (month == 1 and number <= 20):
  print("Козерок")
```

## Задание №4

К следующей лекции прочитать про циклы [for](https://foxford.ru/wiki/informatika/tsikl-for-v-python) и
[while](https://foxford.ru/wiki/informatika/tsikl-while-v-python).

---

Инструкция по выполнению домашнего задания:

1. Зарегистрируйтесь на сайте [Repl.IT](https://repl.it/).
2. Перейдите в раздел **my repls**.
3. Нажмите кнопку **Start coding now!**, если приступаете впервые, или **New Repl**, если у вас уже есть работы.
4. В списке языков выберите Python.
5. Код пишите в левой части окна.
6. Посмотреть результат выполнения файла можно, нажав на кнопку **Run**. Результат появится в правой части окна.

_Никаких файлов прикреплять не нужно._

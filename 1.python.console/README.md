# Домашнее задание к лекции 1.«Python. Знакомство с консолью»

Привет! <br>
Это ваши первые задачи на курсе «Основы языка программирования Python».

После каждой лекции у вас будет 2-3 задачи для самостоятельного решения — ваше домашнее задание. Чтобы выполнить домашнее задание, вам потребуются как знания, которые вы получили из лекционного материала, так и навык поиска информации в интернете — самый важный навык программиста!

Первая задача выполняется на сайте [hackerrank](https://www.hackerrank.com) и проверяется автоматически. Здесь вы можете решать задачи в течение всего курса.
Вторая и третья задачи выполняются на сайте [Repl.IT](https://repl.it/), инструкцию по его использованию вы найдете внизу этой страницы.

## Задача №1

Для успешного выполнения задачи вам нужно:

Зарегистрироваться на сайте [hackerrank](https://www.hackerrank.com).  
Решить задачу ["Say "Hello, World!" With Python"](https://www.hackerrank.com/challenges/py-hello-world/problem).  
Решить задачу ["Arithmetic Operators"](https://www.hackerrank.com/challenges/python-arithmetic-operators/problem).  
Если вам нужна ссылка на ваше решение, на сайте [hackerrank](https://www.hackerrank.com) в правом верхнем углу нажмите на своё имя, перейдите в раздел "Profile" и скопируйте ссылку из адресной строки браузера.

Пример: ссылка на аккаунт eshmargunov - hackerrank.com/eshmargunov

## Ответ

["Say "Hello, World!" With Python"](https://www.hackerrank.com/challenges/py-hello-world/problem?isFullScreen=true)

```
print("Hello, World!")

```

["Arithmetic Operators"](https://www.hackerrank.com/challenges/python-arithmetic-operators/problem?isFullScreen=true)

```
a = int(input())
b = int(input())
print(a + b)
print(a - b)
print(a * b)
```

## Задача №2

Квадрат и прямоугольник.

_Ознакомьтесь с инструкцией по выполнению домашнего задания внизу страницы._

Пользователь вводит длину и ширину фигуры.  
Программа выводит их периметр и площадь.

Пример:

```
Введите длину стороны квадрата: 3

Вывод:
Периметр: 12
Площадь: 9

Введите длину прямоугольника: 3
Введите ширину прямоугольника: 4

Вывод:
Периметр: 14
Площадь: 12
```

Программа запрашивает у пользователя длину стороны квадрата и выводит его периметр и площадь. Сразу после этого пользователю предлагается ввести длину и ширину прямоугольника, для которого рассчитывается периметр и площадь.
Обратите внимание, что программа должна работать корректно при любых введённых значениях длины и ширины фигуры.

## Ответ

```
a = int(input("Введите длину стороны квадрата: "))
print("Периметр:", a * 4)
print("Площадь", a * a)

b = int(input("Введите длину прямоугольника: "))
c = int(input("Введите ширину прямоугольника: "))
print("Периметр прямоугольника:", 2 * ( b + c ))
print("Площадь прямоугольника:", b * c)
```

## Задача №3

Нужно разработать приложение для финансового планирования.  
Приложение учитывает, какой процент от заработной платы уходит на ипотеку и ежемесячные расходы.

Для этого пользователю предлагается ввести следующие данные:

1. Заработную плату в месяц.
2. Какой процент(%) от зп уходит на ипотеку.
3. Какой процент(%) от зп уходит "на жизнь".

Программа подсчитывает и выводит, сколько денег тратит пользователь на ипотеку и сколько он накопит за год (остаток от заработанной платы).

Пример:

```
Введите заработную плату в месяц: 100000
Введите, какой процент(%) уходит на ипотеку: 30
Введите, какой процент(%) уходит на жизнь: 50

Вывод:
На ипотеку было потрачено: 360000 рублей
Было накоплено: 240000 рублей
```

## Ответ

```
a = int(input("Введите заработную плату в месяц: "))
b = int(input("Введите, какой процент(%) уходит на ипотеку: "))
c = int(input("Введите, какой процент(%) уходит на жизнь: "))
d = int(input('Введите, за сколько месяцев (по умолчанию, 12): ').strip() or "12")
print("На ипотеку было потрачено: ", a // 100 * b * d)
print("Было накоплено: ", ((a * d) - ((a // 100 * c * d) + (a // 100 * b * d))))
```

---

Инструкция по выполнению домашнего задания:

1. Зарегистрируйтесь на сайте [Repl.IT](https://repl.it/).
2. Перейдите в раздел **my repls**.
3. Нажмите кнопку **Start coding now!**, если приступаете впервые, или **New Repl**, если у вас уже есть работы.
4. В списке языков выберите Python.
5. Код пишите в левой части окна.
6. Посмотреть результат выполнения файла можно, нажав на кнопку **Run**. Результат появится в правой части окна.

_Никаких файлов прикреплять не нужно._

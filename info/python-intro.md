# Основные конструкции в Python

* [Условия (if ... elif ... else)](#условия-if--elif--else)
  * [If](#if)
  * [Elif](#elif)
  * [Else](#else)
* [Циклы](#циклы)
  * [While](#while)
  * [For](#for)
  * [Операторы цикла](#операторы-цикла)
    * [Continue operator](#continue)
    * [Break operator](#break)

## Условия (if ... elif ... else)
### Логические операторы из математики, которые могут использоваться в Python:

|                   |           |
|-------------------|-----------|
| Равно             | a == b    |
| Не равно          | a != b    |
| Меньше            | a < b     |
| Меньше либо равно | a <= b    |
| Больше            | a > b     |
| Больше либо равно | a >= b    |


### If
Запускает блок кода после условия только если условие оказалось верным.

```python
 Ok
a = 33
b = 200
if b > a:
  print("b is greater than a")
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_if2)


### Elif
Ключевое слово `elif` - это способ python сказать: «Если предыдущие условия не были выполнились, попробуйте проверить это условие».

```python
a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_if_elif)

### Else 
Ключевое слово `else` перехватывает все, что не прошло предыдущие условиями.
```python
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_if_else)


## Циклы 
### While
С помощью цикла `while` мы можем выполнять блок кода, пока выполняется условие.
```python
i = 1
while i < 6:
  print(i)
  i += 1
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_while)


### For
Цикл `for` используется для перебора последовательности. Это может быть список, строка(как последовательность символов). 
```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
 напечатает все фрукты по порядку
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_for)

```python
for x in "banana":
  print(x)
 напечатает все буквы слова по порядку
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_for_string)

В Python, чтобы пройтись в цикле определенное количество раз мы можем использовать функцию range().
Функция range () возвращает последовательность чисел, начиная с 0 по умолчанию и увеличивая на 1 (по умолчанию) и заканчивая указанным числом.

```python
for x in range(6):
  print(x)
 напечатает числа от 0 до 5(!) включительно
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_for_range)
>Обратите внимание, что range(6) - это не значения от 0 до 6, а *значения от 0 до 5*.

## Операторы цикла
### Continue
С помощью оператора continue мы можем остановить текущую итерацию и продолжить следующую.
```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    continue
  print(x)
 не напечатает только "banana"
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_for_continue)


```python
i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
 не напечатает 3
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_while_continue)

### Break
С помощью оператора `break` мы можем остановить цикл до того, как он пройдёт через все элементы.
```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
 напечатает только "apple" и "banana"
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_for_break)


```python
i = 1
while i < 6:
  print(i)
  if i == 3:
    break
  i += 1
 напечатает только 1, 2 и 3
```
[Запустить самому](https://www.w3schools.com/python/trypython.asp?filename=demo_while_break)


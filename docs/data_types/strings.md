# Строки

Строки - это тестовый тип данных Python

Для того чтобы создать строки в буквальном виде, нужно использовать кавычки. Подойдут одинарные, двойные так и тройные:
```py
# 4 разных способа создания строк
print('hello', "hello", """"hello""", '''hello''')
```
Тройные кавычки позволяют создавать значения используя несколько строк
```py
'так
нельзя
это вызовет ошибку'

'''
а так
можно
ошибки не будет
'''
```

## Операции над строками

```py
# Сложение
# В результате строки "склеиваются" в одну большую строку
>>> print('Hello' + ' ' + 'world')
Hello world
>>> print('2' + '2')
22

# Умножение на число создает новую строку 
# состоящую из повторения предыдущей
>>> print('Sergey' * 4)
SergeySergeySergeySergey
```

## Итерация

По строкам можно итерировать также как и по спискам:
```py
string = 'Hello there'

# Цикл for с использованием range
for i in range(len(string)):
    print(string[i])

# Цикл for без range

for char in string:
    print(char)
```


## Индексация

Для индексации строк используют квадратные скобки [] и число выступающие индексом.
Начало индексации всегда с нуля. Таким образом, если строка состоит из n 

```py
>>> string = 'Hello world'
# Первый символ
>>> print(string[0])
H
# Последний символ
>>> print(string[-1])
d
# Подстроки
>>> print(string[:3])
Hel
>>> print(string[3:])
lo world
>>> print(string[3:5])
lo
# Лаконичный способ перевернуть строку
>>> print(string[::-1])
dlrow olleH
```

## Встроенные методы


| Метод                            | Что делает                                                                               |
| -------------------------------- | ---------------------------------------------------------------------------------------- |
| **split**(sep)                   | Разбивает строку по определенному разделителю(sep). Возвращает список состоящий из строк |
| **strip**()                      | Убирает знаки пробела и табуляции с двух концов. Возвращает строку                       |
| **lower**/**upper**()            | Переводит строку в нижний(lower) или верхний(upper) регистр                              |
| **replace**(substr, repl_substr) | Заменяет одну подстроку(substr) другой(repl_substr)                                      |
| **isdigit**()                    | Возвращает является ли строка цифрой(True/False)                                         |
| **count**()                      | Возвращает встречаемость подстроки в строке                                              |

1. **split** 
```py
>>> string = 'Мой номер телефона: +799999999'
>>> print(string.split(' '))
['Мой', 'номер', 'телефона:', '+799999999']
>>> print(string.split(':'))
['Мой номер телефона', ' +799999999']
>>> print(string.split('+'))
['Мой номер телефона: ', '799999999']
```
1. **strip** 
```py
>>> string = ' лишний пробел слева'
>>> print(string.strip())
лишний пробел слева
>>> string = 'лишний пробел справа '
>>> print(string.strip())
лишний пробел справа
>>> string = '  лишний пробелы везде  '
>>> print(string.strip())
лишний пробелы везде
```
1. **lower/upper**
```py
>>> string = 'Буквы'
>>> print(string.lower())
буквы
>>> print(string.upper())
БУКВЫ
```
1. **replace** 
```py
>>> string = 'Бук в ы'
>>> print(string.replace(' ', ''))
Буквы
>>> print(string.replace('Бук', '^__^'))
^__^ в ы
```
1. **isdigit**
```py
>>> print('45'.isdigit())
True
>>> print('45.5'.isdigit())
False
>>> print('Hello'.isdigit())
False
```
1. **count**
```py
print('HHHHhhho'.count('h'))
3
print('HHHHhhho'.count('HH'))
2
print('HHHHhhho'.count('O'))
0
```
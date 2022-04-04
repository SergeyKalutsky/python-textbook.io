# for

Цикл **for** в питоне используеся для итерации по какой-либо коллекции (список, кортеж, словарь, множество, [строки](../data_types/strings.md))

### Синтаксис

```py
for variable in iterable:
    #code
```

1. Ключевые слова **for** и **in** обязательны
2. variable - любая переменная(см. [правила названия переменны](../index.md))

```py
>>> fruits = ["яблоко", "банан", "вишня"]
>>> for x in fruits:
>>>   print(x)
яблоко
банан
вишня
```
Цикл **for** можно использовать и для [строк](../data_types/strings.md):
```py
>>> for x in "hello world":
>>>  print(x)
h
e
l
l
o
 
w
o
r
l
d
```

Цикл **for** часто используется со встроенной функцией [range](../built_ins/range.md)

# Комментарии 

Коментарии начинаются с **#** и **Python** интерпритатор игнорирует их 

```py
# Это комментарий
print("Hello, World!")

print('Hi') # И это комментарий
```
В коментарии можно писать что угодно, **Python** проигрнорирует этот текст

```py
#print("Мена не напечатают :(")
print("А меня напечатают")
```

В языке Python в отличие от многих других отсутствуют многострочные комментарии. Иногда для этих целей используют [строки](data_types/strings.md)
```py
'''
Это многострочный комментарий
который на самом деле не комментарий
а просто строка, не присвоенная на переменную
'''
print('hello world')
```
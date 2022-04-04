# Boolean

Тип данных **Boolean** состоит из двух значений **True**(Истинно) и **False**(Ложно)
```py
>>> print(type(True))
<class 'bool'>
>>> print(type(False))
<class 'bool'>
```
В питоне все может выступать в роли **Boolean**. Чтобы посмотреть, какое значение **Boolean** примет то или иной значение используйте 
встроенный метод **bool**:
```py
# Все числа кроме нуля принимают значение True, 0 принимает False
>>> print(bool(1))
True
>>> print(bool(0))
False

# Все не пустые строки принимают значение True
>>> print(bool('Hmm'))
True
>>> print(bool(''))
False
```
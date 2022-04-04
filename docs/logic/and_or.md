# and и or

**and** и **or** позволяют объединять несколько условий

При этом  **and** -  это строгий оператор. В результате будет True, только если все значения True

**or** - не строгий оператор и возврщает True, если хотя бы одно условие истинно
```py
>>> print(True and True and True and False)
False
>>> print(True or True or True or False)
True
```
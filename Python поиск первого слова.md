###### Time: 23:13  15-06-23  
###### Tags:  #python #programmingproblems
###### ZeroLinks: [[00 it]]
###### Links: 

[First Word (simplified)](https://py.checkio.org/ru/mission/first-word-simplified/)

```python
def first_word(text: str) -> str:
    return text.split()[0]

```

решение быстрее
```python
def first_word(text):
    index = text.find(" ")
    return text[:index] if index != -1 else text
```

Метод `text.find(" ")` и `text[:index]` используют метод `find()`, чтобы найти индекс первого пробела в строке, и затем возвращают срез строки до этого индекса. Этот метод не создает промежуточный список и может быть немного быстрее при обработке очень длинных строк.

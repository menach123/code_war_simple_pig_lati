
### <a href=https://www.codewars.com/kata/520b9d2ad5c005041100000f/train/python>Simple Pig Latin</a>

Move the first letter of each word to the end of it, then add "ay" to the end of the word. Leave punctuation marks untouched.

#### Examples
```
pig_it('Pig latin is cool') # igPay atinlay siay oolcay
pig_it('Hello world !')     # elloHay orldway !
```


```python
def pig_it(text):
    
    
    return ' '.join([word[1:]+ word[0]+ 'ay' if word[0] not in ',./?!*-_' else word for word in text.split(' ')])
```


```python
pig_it('Pig latin is cool')
```




    'igPay atinlay siay oolcay'




```python
pig_it('Hello world !')
```




    'elloHay orldway !'




```python
pig_it('This is my string') #'hisTay siay ymay tringsay'
```




    'hisTay siay ymay tringsay'




```python

```

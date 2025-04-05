---
jupyter:
  jupytext:
    formats: ipynb,md
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.16.7
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
---

<!-- #region slideshow={"slide_type": "slide"} -->
# Expressions

Let's start with some basic expressions. To execute the code online you can open the file in google colab by clicking the colab button below or rocket button above.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/code4geoai/pythonic/blob/main/book/PartI/Expressions.ipynb)

<!-- #endregion -->

## How to execute the code
When you open the file in colab and select the cell having code and press Ctl/Command + Enter. The code will be executed and you will see the output below the cell. Lets try some basic arithmetic expressions.

```python
17
```

```python slideshow={"slide_type": "fragment"}
-2 + 15
```

```python
-2 - 1 
```

```python
-2 -     -1 
```

### Division `/`

```python slideshow={"slide_type": "slide"}
14 / 3 
```

```python
1 / 2
```

### Modulus or Reminder Operator `%`

```python
1 % 2
```

```python
15 % 2
```

```python slideshow={"slide_type": "slide"}
1 / 2.0
```

### Checking datatype of a number

```python
type(1) 
```

```python
type(1/2.0 + 1/4.0) 
```

```python slideshow={"slide_type": "slide"}
2.1 + 5.3
```

```python
2 + 2 * 2
```

```python
(2 + 2) * 2 # overriding precedence
```

<!-- #region slideshow={"slide_type": "slide"} -->
See more about precedence here: https://docs.python.org/3/reference/expressions.html#operator-precedence
<!-- #endregion -->

### Conditional Expression

```python slideshow={"slide_type": "slide"}
3 < 4       
```

```python
3 == 4
```

```python slideshow={"slide_type": "slide"}
3 == 3 
```

```python
3 = 3   # ignore the *details* of the error for now
```

```python
3 > 4 
```

```python jupyter={"outputs_hidden": true} slideshow={"slide_type": "slide"}
3 >= 3 
```

```python jupyter={"outputs_hidden": true}
2 <= 1
```

<!-- #region slideshow={"slide_type": "slide"} -->
### Other types of expressions 
<!-- #endregion -->

```python
'abc'
```

```python jupyter={"outputs_hidden": true}
"xyz"
```

```python jupyter={"outputs_hidden": true}
"""This is called a multi-line string.     
It can, obviously, span multiple lines! """
```

```python slideshow={"slide_type": "slide"}
"ab" + "cd"
```

```python
type("ab")
```

```python
"a-" * 3
```

```python jupyter={"outputs_hidden": true}
True
```

```python jupyter={"outputs_hidden": true}
False 
```

```python slideshow={"slide_type": "slide"}
True and True 
```

```python jupyter={"outputs_hidden": true}
True and False 
```

```python jupyter={"outputs_hidden": true}
False and True 
```

```python jupyter={"outputs_hidden": true}
False and False 
```

```python jupyter={"outputs_hidden": true} slideshow={"slide_type": "slide"}
True or True 
```

```python jupyter={"outputs_hidden": true}
True or False 
```

```python jupyter={"outputs_hidden": true}
False or True
```

```python jupyter={"outputs_hidden": true}
False or False 
```

```python jupyter={"outputs_hidden": true} slideshow={"slide_type": "slide"}
True or False and False or False 
```

```python jupyter={"outputs_hidden": true}
(True or False) and (False or False)
```

<!-- #region slideshow={"slide_type": "slide"} -->
### Call Expressions 
<!-- #endregion -->

```python
max(7, 9)
```

```python jupyter={"outputs_hidden": true}
max(2+25, 9) 
```

```python jupyter={"outputs_hidden": true} slideshow={"slide_type": "fragment"}
pow(3, 2)
```

```python jupyter={"outputs_hidden": true} slideshow={"slide_type": "slide"}
max( min(1, -2) , min( pow(3, 5) , -4) )
```

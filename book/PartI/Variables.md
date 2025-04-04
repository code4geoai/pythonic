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
# Variables 
<!-- #endregion -->

<!-- #region slideshow={"slide_type": "slide"} -->
### Naming the numbers 

In Python, a variable is a symbolic name that 
1. Refers to a value stored in memory.
2. Is dynamically typed (no explicit type declaration needed).
3. Can be reassigned to different values/objects.
<!-- #endregion -->

```python
x = 24
```

```python
x
```

```python
x = 3
```

```python
x = 2.0 
```

```python slideshow={"slide_type": "slide"}
y = x * 2
```

```python
y
```

```python
type(y)
```

```python
y * 3
```

### Importing Variables from Library

```python
from math import pi 
```

```python jupyter={"outputs_hidden": true}
pi
```

```python jupyter={"outputs_hidden": true}
pi * 4 * 4  # area of a circle with radius 4cm
```

```python jupyter={"outputs_hidden": true}
radius = 4
```

```python jupyter={"outputs_hidden": true}
pi * pow(radius, 2)
```

```python jupyter={"outputs_hidden": true} slideshow={"slide_type": "slide"}
a = 4
b = 2
pi * pow(a, b) 
```

<!-- #region slideshow={"slide_type": "slide"} -->
What happens when you try to use a variable that is not defined.
<!-- #endregion -->

Let's discuss this in detail. 

<!-- #region slideshow={"slide_type": "slide"} -->
### Naming functions 
Line naming  numbers you can also name functions. If we use a variable without defining it, system will show an error.
<!-- #endregion -->

```python
f
```

```python
from math import sqrt 
```

```python
sqrt(25) 
```

```python
sqrt 
```

** As shown above sqrt is a function in math library lets name it f as shown below.**

```python slideshow={"slide_type": "slide"}
f = sqrt
```

```python
sqrt(25)
```

```python
f(25) 
```

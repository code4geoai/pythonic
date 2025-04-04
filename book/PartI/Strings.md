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

# [Strings](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)

```python
my_string = "Python is my favorite programming language!"
```

```python
my_string
```

```python
type(my_string)
```

```python
len(my_string)
```

### Respecting [PEP8](https://www.python.org/dev/peps/pep-0008/#maximum-line-length) with long strings

```python
long_story = (
    "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
    "Pellentesque eget tincidunt felis. Ut ac vestibulum est."
    "In sed ipsum sit amet sapien scelerisque bibendum. Sed "
    "sagittis purus eu diam fermentum pellentesque."
)
long_story
```

## `str.replace()`


If you don't know how it works, you can always check the `help`:

```python
help(str.replace)
```

This will not modify `my_string` because replace is not done in-place.

```python
my_string.replace("a", "?")
print(my_string)
```

You have to store the return value of `replace` instead.

```python
my_modified_string = my_string.replace("is", "will be")
print(my_modified_string)
```

## f-strings

```python
first_name = "John"
last_name = "Doe"
age = 88
print(f"My name is {first_name} {last_name}, you can call me {first_name}.")
print(f"I'm {age} years old.")
```

```python
print(f"Use '=' to also print the variable name like this: {age=}")
```

## `str.join()`

```python
pandas = "pandas"
numpy = "numpy"
requests = "requests"
cool_python_libs = ", ".join([pandas, numpy, requests])
```

```python
print(f"Some cool python libraries: {cool_python_libs}")
```

Alternative (not as [Pythonic](http://docs.python-guide.org/en/latest/writing/style/#idioms) and [slower](https://waymoot.org/home/python_string/)):

```python
cool_python_libs = pandas + ", " + numpy + ", " + requests
print(f"Some cool python libraries: {cool_python_libs}")

cool_python_libs = pandas
cool_python_libs += ", " + numpy
cool_python_libs += ", " + requests
print(f"Some cool python libraries: {cool_python_libs}")
```

## `str.upper(), str.lower(), str.title()`

```python
mixed_case = "PyTHoN hackER"
```

```python
mixed_case.upper()
```

```python
mixed_case.lower()
```

```python
mixed_case.title()
```

## `str.strip()`

```python
ugly_formatted = " \n \t Some story to tell "
stripped = ugly_formatted.strip()

print(f"ugly: {ugly_formatted}")
print(f"stripped: {stripped}")
```

## `str.split()`

```python
sentence = "three different words"
words = sentence.split()
print(words)
```

```python
type(words)
```

```python
secret_binary_data = "01001,101101,11100000"
binaries = secret_binary_data.split(",")
print(binaries)
```

## Calling multiple methods in a row

```python
ugly_mixed_case = "   ThIS LooKs BAd "
pretty = ugly_mixed_case.strip().lower().replace("bad", "good")
print(pretty)
```

Note that execution order is from left to right. Thus, this won't work:

```python
pretty = ugly_mixed_case.replace("bad", "good").strip().lower()
print(pretty)
```

## [Escape characters](http://python-reference.readthedocs.io/en/latest/docs/str/escapes.html#escape-characters)

```python
two_lines = "First line\nSecond line"
print(two_lines)
```

```python
indented = "\tThis will be indented"
print(indented)
```

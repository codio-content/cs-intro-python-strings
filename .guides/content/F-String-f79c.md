----------

## F-String

F-strings are a feature of Python versions 3.6 and above. F-strings are an evolution of the `format` method and simplify the process of string interpolation. F-strings start with the letter `f` followed by the string. Use `{}` to insert a variable, but put the variable between the `{}`.

![F-Strings](.guides/images/f-strings.png)

<details>
  <summary><strong>What does the "f" mean?</strong></summary>
  The "f" stands for fast. F-strings are executed faster than any other form of string interpolation. Here is an <a href="https://realpython.com/python-f-strings/#speed">article</a> about f-strings that shows the time differences for various forms of string interpolation.
</details>

```python
var1 = "Up"
var2 = "away"
my_string = f"{var1}, up and {var2}."
print(my_string)
```

{try it}(python3 code/strings/f-strings.py 1)

|||challenge
## What happens if you:
* Change the value of `var1` to `7`?
* Change the first `{}` to `{var1 + 10}`?
* Change the second `{}` to `{var2.upper()}`?

|||

{try it}(python3 code/strings/f-strings.py 2)

## Multi-line F-Strings

You can use the same ideas from the lesson on multi-line strings to make multi-line f-strings. 

```python
name = "Calvin"
age = 6
occupation = "student"
sentence = f"My name is {name}. " \
           f"I am {age} years old. " \
           f"I am a {occupation}."
print(sentence)
```

{try it}(python3 code/strings/f-strings.py 3)

|||challenge
## What happens if you:
Use the `"""` method for multi-line strings?
```python
name = "Calvin"
age = 6
occupation = "student"
sentence = f"""My name is {name}.
I am {age} years old.
I am a {occupation}."""
print(sentence)
```

|||

{try it}(python3 code/strings/f-strings.py 4)

<details>
  <summary><strong>Use the appropriate number of <code>f</code>'s</strong></summary>
  The <code>\</code> method for making multi-line strings requires that you put an <code>f</code> before each set of quotation marks. The <code>"""</code> method for making multi-line strings requires only one <code>f</code> before the <code>"""</code>. That is because there is only one set of <code>"""</code>. Be sure that you have an <code>f</code> for each set of quotation marks when making multi-line strings.
</details>

{Check It!|assessment}(fill-in-the-blanks-2634811268)

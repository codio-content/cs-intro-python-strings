----------

## Formatting Strings with %

**Important:** Formatting strings with `%` is **not** the recommended way for string interpolation in Python 3. The `%` operator was commonly used for string interpolation, and has a similar syntax as the `format` method for string interpolation.

![Old String Interpolation](.guides/images/old-string-interpolation.png)

```python
var1 = "Up"
var2 = "away"
print("%s, up and %s" % (var1, var2))
```

{try it}(python3 code/strings/old-string-interpolation.py 1)

<details>
  <summary><strong>What does the <code>s</code> in <code>%s</code> mean?</strong></summary>
  The <code>s</code> means that the variable that will go in this position will be a string. If <code>var1</code> is an integer, use <code>%i</code>. If it is a float, use <code>%f</code>.
</details>

|||challenge
## What happens if you:
* Swap the position of `var1` and `var2`?
* Remove the `s` from the `%`?
* Change `var1` to `7` and change the first `%s` to `%i`?

|||

{try it}(python3 code/strings/old-string-interpolation.py 2)

## Why Learn the Old Way?

Python was first released in 1991. Python 3 was not released until 2008. Even then, many developers were slow to adopt Python 3. Because of this, so many examples of Python that you will see in books, websites, and videos will use `%` for string interpolation. You should be able to read and understand this code. However, you should write code using modern methods of string interpolation. 

{Check It!|assessment}(fill-in-the-blanks-3263461860)


This file tests various uses of the code-cell directive.

First, a simple code-cell:

```{code-cell} python
x = 1
assert x == 1
```

Now a code-cell with doctest:

```{code-cell} python
>>> 2 + 2
4
```

And a code-cell that uses previously defined variables:

```{code-cell} python
y = x + 1
assert y == 2
```

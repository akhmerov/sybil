Testing invisible code-cell blocks.

First, a regular code-cell:

```{code-cell} python
x = 1
```

Now an invisible code-cell in percent comment style:

% invisible-code-cell: python
%
% y = 2
% assert y == 2

And an invisible code-cell in HTML comment style:

<!--- invisible-code-cell: python
z = 3
assert z == 3
--->

Finally, verify all variables are accessible:

```{code-cell} python
assert x == 1
assert y == 2
assert z == 3
```

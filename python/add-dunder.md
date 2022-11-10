---
description: 10th November 2022
---

# add dunder

\- `__add__` should be used if you want to create a new object.&#x20;

\- `__iadd__` should be used if you want to modify the existing item in which case you should use `x += y` instead of `x = x + y`.&#x20;

\- Both need to `return` the result that you want them to be.

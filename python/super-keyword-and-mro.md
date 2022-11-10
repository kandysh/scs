---
description: 10th November 2022
---

# super keyword and MRO

`super()` in python only cares about the method resolution order. Consider an example

{% code overflow="wrap" %}
```python
class A:
    def __init__(self):
        print("A")
class B(A):
    def __init__(self):
        print("B")
        super().__init__()

class C:
    def __init__(self):
        print("C")
        super().__init__()

class D(B, C):
    def __init__(self):
        print("D")
        super().__init__()

print([cls.__name__ for cls in D.__mro__])
d=D()
```
{% endcode %}

```python
>>> D B A C object
>>> D B A 
```

as per the rules of multiple inheritance first parent's init is called then their super's and their super's. The super chain stops at A as it has no super method. (And it makes no sense to add a super call from A as it is the parent class). But what if we add a super init call to A too&#x20;

```python
class A:
    def __init__(self):
        print("A")
        super().__init__()
```

```python
>>> D B A C object
>>> D B A C
```

This shows A's super called C. Super method never cares about the class's inheritance it cares about the MRO of a certain class. This a weird behaviour but is implemented to overcome diamond problem.

More about how MRO is created can be read in the documentation.\

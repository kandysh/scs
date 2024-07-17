---
description: Seventh, October 2022
---

# Ways to inherit a class

Inheritance can be done in three ways in python

{% code overflow="wrap" %}
```python
class Base():
    def __init__(self):
        print ("Base created")
        
class ChildA(Base):
    def __init__(self):
        Base.__init__(self)
        
class ChildB(Base):
    def __init__(self):
        super(ChildB, self).__init__()

class ChildC(Base):
    def __init__(self):
        super().__init__()
```
{% endcode %}

The second and third methods are the same as super passes class name and self implicitly.\
`super(ChildB,self)=super()`.\
Now coming to the difference in the two methods, the first one runs the Base classes init method but never follows the MRO, but when we do `super().__init__()` then it follows Class C's MRO.

The only noticeable difference can be seen in multiple inheritance.

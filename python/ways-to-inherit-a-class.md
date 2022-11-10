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

Here the class B and C are equal and that's how super works on it's own, more can be read about that in the python `super()` docs.

Now in the se . MRO&#x20;

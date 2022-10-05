---
description: Fifth, October 2022
---

# Craziest rock paper scissor

Using walrus and string slicing we can write the rock paper scisssor logic in one-line, though not recommended.

{% code overflow="wrap" %}
```python
for _ in [0]*int(input('Number of rounds?')):print((c:=("Rock","Paper","Scissors"))[(u:=int(input(f"0.Rock 1.Paper 2.{c[2]}")))],c[(a:=__import__('random').randrange(3))],"tuaisiee  r"[(u-a)%3::3])
```
{% endcode %}

_code is taken from programmers' hangout_

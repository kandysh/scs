---
description: Fifth, October 2022
---

# Craziest rock paper scissor



{% code overflow="wrap" %}
```python
for _ in [0]*int(input('Number of rounds?')):print((c:=("Rock","Paper","Scissors"))[(u:=int(input(f"0.Rock 1.Paper 2.{c[2]}")))],c[(a:=__import__('random').randrange(3))],"tuaisiee  r"[(u-a)%3::3])
```
{% endcode %}

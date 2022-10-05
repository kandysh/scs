---
description: Fifth, October 2022
---

# Exclusive strings matching

This is a follow-up of the [.](./ "mention")where we might not need the first and second strings.

In that case, we use a `?: non-capturing group` character, so the regex matches the pattern but never groups it for our result.\


### Single line

```regex
(?:first_string)(.*?)(?:second_string)
```

### Multi-line

```regex
(?:first_string)((.|\n)*?)(?:second_string)
```

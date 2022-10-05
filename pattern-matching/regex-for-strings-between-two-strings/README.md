---
description: Fifth, October 2022
---

# Regex for strings between two strings

We may find a case to match strings between two strings inclusively.

### Single-line

```regex
(first_string)(.*?)(second_string)
```

`.*` looks for characters and `?` makes it there can be characters or not.

### Multi-line

```regex
(first_string)((.|\n)*?)(second_string)
```

here the with the addition of `|`and `\n` we add a case to check for new lines.&#x20;

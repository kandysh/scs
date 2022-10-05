---
description: Fifth, October 2022
---

# Variable-naming patterns



| Pattern                                 |  Example  | Meaning                                                                                                                                                                            |   |
| --------------------------------------- | :-------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | - |
| SIngle Leading Underscore               |   `_var`  | Naming convention indidcating a name is meant for internal use. Generally not enforced by the interpreter(unless wildcard imports) and meant to just give hints to the programmer. |   |
| Single Trailing Underscore              |   `var_`  | Used to avoid conflicts with python keywords.                                                                                                                                      |   |
| Double leading Underscore               |  `__var`  | Triggers name mangling when used in class context.                                                                                                                                 |   |
|                                         |           |                                                                                                                                                                                    |   |
| Double leading and trailing Underscore  | `__var__` | Indicates special methods defined by Python languages. Avoid this naming scheme for your variables.                                                                                |   |
| Single Underscore                       |     \_    | Used as a placeholder for insignificant variables. Also gives you the last variable in python REPL.                                                                                |   |

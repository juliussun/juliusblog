---
author: Julius
pubDatetime: 2024-03-23T21:38:53.000Z
modDatetime: 
title: How python import modules
featured: false
draft: true
tags:
  - python
description: A close look into python's import mechanism
---

Have you ever wondered why we need to use \_\_init\_\_.py file in python? Or ran into some weird issues of `module not found` ? Well, I am. I decided to take a closer look at why and how.

>  namespace is fundamental to any programming languages. It is a way for computer to make sure that there is no ambiguity or conflict when we call any combinations of identifiers. It usually consist of variable names, function names, class names, etc.
### Namespace in Python

In python, a namespace is a mapping of objects with names. The main categories are:
- local
- global
- built-in
- modules

![[Pasted image 20240323215947.png]]
*figure credit: programiz.com

Python's import of modules or packages looks like this:
```python
import module_A
```

Python runtime will follow a sequences of steps to deal with the import.
1. It will try to search directories in the `sys.path` (where your python env sits)

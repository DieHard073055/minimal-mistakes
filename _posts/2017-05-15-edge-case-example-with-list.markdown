---
title: "Edge Case: Nested and Mixed Lists"
categories:
  - Edge Case
tags:
  - content
  - css
  - edge case
  - lists
  - markup
header:
  image: https://farm5.staticflickr.com/4140/4939863887_84705982fd_b.jpg
---

Nested and mixed lists are an interesting beast. It's a corner case to make sure that

* Lists within lists do not break the ordered list numbering order
* Your list styles go deep enough.

### Ordered -- Unordered -- Ordered

1. ordered item
2. ordered item
  * **unordered**
  * **unordered**
    1. ordered item
    2. ordered item
3. ordered item
4. ordered item

### Ordered -- Unordered -- Unordered

1. ordered item
2. ordered item
  * **unordered**
  * **unordered**
    * unordered item
    * unordered item
3. ordered item
4. ordered item

### Unordered -- Ordered -- Unordered

* unordered item
* unordered item
  1. ordered
  2. ordered
    * unordered item
    * unordered item
* unordered item
* unordered item

### Unordered -- Unordered -- Ordered

* unordered item
* unordered item
  * unordered
  * unordered
    1. **ordered item**
    2. **ordered item**
* unordered item
* unordered item

```python
def awesome():
  print( "Well here is awesome!" )

if __name__ == '__main__':
  awesome() # Hope this works

```

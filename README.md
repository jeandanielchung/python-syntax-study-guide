# python-syntax-study-guide
## Arrays

### Instatiation
`l = []`

`l = [3, 6, 2]`

### List comprehension
`l = [a for a in range(10) if a % 2 == 0]`

### Indexing/Slicing
**Indexing**

`elem = l[4]` (get 4th element in 0-indexed list)

`elem = l[-1]` (get last element in list)

**Slicing**

*Note that slicing returns a new shallow copy of the list*
`elems = l[1:3]`

`elems = l[:2]`

`elems = l[4:]`

`elems = l[-1:-1:-1]`

### Functions

**Sorting**

`l_sorted = sorted(l)` (creates new list)

`l.sort()` (in-place)

`l_sorted_desc = sorted(l, reverse=True)`

`l_sorted_key = sorted(l, key=lambda x:(x % 2, x)` (sort by even numbers first then ascending order)

**Reversing**

`elems = l[-1:-1:-1]`

`l_reversed = reversed(l)`

`l.reverse()`

**Appending**

`l.append(2)`

`l.extend([3, 1, 6])`


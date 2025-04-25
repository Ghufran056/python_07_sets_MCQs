
### 1. The items of set are?
A. `mutable`  
B. `immutable`  
C. `ordered`  
D. `both c & d`  
<details>
<summary>Answer</summary>
B. `immutable` — the items of set are immutable but the set itself is mutable
</details>

### 2. What will be the output?
```python
my_set: set = set([123, (4, 50), 45, 5]) 
print(my_set)
```
A. `{123, 4, 50, 45, 5}`  
B. `[(4, 50), 123, 45, 5]`  
C. `{123, (4, 50), 45, 5}`  
D. `TypeError`  
<details>
<summary>Answer</summary>
C. `{123, (4, 50), 45, 5}`
</details>

### 3. What will be the output?
```python
my_set: set = {}
print(type(my_set))
```
A. `<class 'set'>`  
B. `<class 'dict'>`  
C. `<class 'NoneType'>`  
D. `{ }`  
<details>
<summary>Answer</summary>
B. `<class 'dict'>`
</details>

### 4. What will be the output of `my_set2`?
```python
my_set = {1,2}
my_set2 = my_set
my_set.add(5)
print(my_set2)
```
A. `{1,2}`  
B. `{1,2,5}`  
C. `{}`  
D. `None`  
<details>
<summary>Answer</summary>
B. `{1,2,5}` — `my_set2` is a reference to `my_set`, so both reflect the same change.
</details>

### 5. What will be the output?
```python
my_set: set = {1,2,[4,5],3}
print(my_set)
```
A. `{1,2,[4,5],3}`  
B. `{1,2,4,5,3}`  
C. `SyntaxError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
D. `TypeError` — because a set can only store immutable elements.
</details>

### 6. What will be the output?
```python
my_set: set = {10,20,30,40,50}
print(my_set[0:2])
```
A. `{10, 20}`  
B. `{10, 20, 30}`  
C. `IndexError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
D. `TypeError` — sets are unordered, so indexing doesn’t work.
</details>

### 7. What will be the output?
```python
my_set: set = {1, 2, 3, 4, 5, 'A', 'a'}
print(my_set.discard({1,2,3}))
```
A. `{4, 5, 'A', 'a'}`  
B. `{1, 2, 3}`  
C. `None`  
D. `KeyError`  
<details>
<summary>Answer</summary>
C. `None` — `discard()` doesn't raise an error and `{1,2,3}` isn’t an element in `my_set`.
</details>

### 8. What will be the output?
```python
my_set: set = {1, 2, 3, 4, 5, 'A', 'a'}
my_set.difference_update({1, 5, 3, 'A'})
print(my_set)
```
A. `None`  
B. `{2, 4, 'a'}`  
C. `TypeError`  
D. `{1, 5, 3, 'A'}`  
<details>
<summary>Answer</summary>
B. `{2, 4, 'a'}` — `difference_update()` removes multiple elements.
</details>

### 9. What's the difference between `discard()` and `remove()` method?
A. `discard()` removes multiple items and `remove()` removes one.  
B. `remove()` raises error if item not found, `discard()` does not.  
C. `discard()` raises error, `remove()` does not.  
D. Both raise error if item not found.  
<details>
<summary>Answer</summary>
B. `remove()` raises error if not found, `discard()` does not.
</details>

### 10. Hashable objects are?
A. `mutable`  
B. `immutable`  
C. `both a & b`  
D. `None`  
<details>
<summary>Answer</summary>
B. `immutable` — only immutable objects are hashable.
</details>

### 11. What will be the output?
```python
my_set: set = {1, 2, 3, 4, 5}
my_set2 = my_set
my_set.add(7)
print(my_set is my_set2)
```
A. `SyntaxError`  
B. `False`  
C. `True`  
D. `None`  
<details>
<summary>Answer</summary>
C. `True` — both variables refer to the same set object.
</details>

### 12. What will be the output?
```python
Set = {1,2,3}
print(hash(Set))
```
A. This will print a hash value  
B. `SyntaxError`  
C. `KeyError`  
D. `TypeError`  
<details>
<summary>Answer</summary>
D. `TypeError` — sets are unhashable because they're mutable.
</details>

### 13. What will be the output?
```python
my_set:  set = {1,2,3, "Hello! World", 4,5,6}
my_set2: set = {1,2,3, "Hello! World", 8,9}
print(my_set.symmetric_difference(my_set2))
```
A. Set difference  
B. Unique items from both  
C. All unique items from both sets  
D. None  
<details>
<summary>Answer</summary>
C. `Return a set that contains only unique items from both sets`
</details>

### 14. What will be the output?
```python
Set = {2,3,5,6,7}
Set2 = Set.copy()
print(Set is Set2)
```
A. `True`  
B. `False`  
C. `TypeError`  
D. `None of them`  
<details>
<summary>Answer</summary>
B. `False` — `.copy()` creates a new object with same values.
</details>

### 15. What will be the output?
```python
frozen_set1: frozenset = frozenset([1, 2, 3, 4])
copy_set: frozenset = frozen_set1.copy()
print(frozen_set1 is copy_set)
```
A. `True`  
B. `False`  
C. `TypeError`  
D. `None of them`  
<details>
<summary>Answer</summary>
A. `True` — `frozenset.copy()` returns the same object (immutable).
</details>

### 16. What happens when an object’s reference count is 0?
A. It stays in memory  
B. Garbage collector frees it  
C. It turns into `None`  
D. Python raises an error  
<details>
<summary>Answer</summary>
B. `The garbage collector free up memory occupied by these objects.`
</details>

### 17. What will be the output?
```python
s = {True, 1, 2}
print(len(s))
```
A. `3`  
B. `2`  
C. `1`  
D. `TypeError`  
<details>
<summary>Answer</summary>
B. `2` — `True` is equal to `1`, so they collapse to one item.
</details>

### 18. What will be the output?
```python
s = {1, 2, 3}
s.update([4], (5,), {6})
print(s)
```
A. `{1, 2, 3, 4, 5, 6}`  
B. `{1, 2, 3, [4], (5,), {6}}`  
C. `TypeError`  
D. `{1, 2, 3}`  
<details>
<summary>Answer</summary>
A. The `update()` method adds elements from all iterables to the set.
</details>

### 19. What will be the output?
```python
a = set("hello")
b = set("world")
print(a & b)
```
A. `{'l', 'o'}`  
B. `{'h', 'e', 'l', 'o', 'w', 'r', 'd'}`  
C. `set()`  
D. `TypeError`  
<details>
<summary>Answer</summary>
A. `{'l', 'o'}` — set intersection of common letters.
</details>

### 20. What will be the output?
```python
print({frozenset({1, 2}), frozenset({2, 1})})
```
A. `{frozenset({1, 2}), frozenset({2, 1})}`  
B. `{frozenset({1, 2})}`  
C. `TypeError`  
D. `None of the above`  
<details>
<summary>Answer</summary>
B. `frozenset({1, 2})` — duplicates are removed as sets are equal.
</details>

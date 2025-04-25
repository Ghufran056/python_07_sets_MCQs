1. the items of set are?
a. `mutable`
b. `immutable`
c. `ordered`
d. `both c & d`
<details>
<summary>answer</summary>
C, (the items of set are immutable but the set is mutable)
</details>

2. What will be the output.
```python
   my_set: set = set([123,(4,50), 45, 5]) 
    print(my_set)
```
a. `{123, 4, 50, 45, 5}`
b. `[(4, 50), 123, 45, 5]`
c. `{123, (4, 50), 45, 5}`
d. `TypeError`
<details>
<summary>answer</summary>
`{123, (4, 50), 45, 5}`
</details>

3. What will be the output?
```python
   my_set: set = {}
   print(type(my_set)) 
```
a. `<class 'set'>`
b. `<class 'dict'>`
c. `<class 'NoneType'>`
d. `{ }`
<details>
<summary>answer</summary>
`<class 'dict'>`
</details>

4. What will be the output of my_set2?
```python
    my_set = {1,2}
    my_set2 = my_set
    my_set.add(5)
    print(my_set2)  
```
a. `{1,2}`
b. `{1,2,5}`
c. `{}`
d. `None`
<details>
<summary>answer</summary>
{1,2,5}, Since my_set2 is a reference to my_set, modifying my_set with .add(5) will also affect my_set2, as they point to the same object in memory.
</details>

5. What will be the output?
```python
   my_set: set = {1,2,[4,5],3}
   print(my_set)
 ```
a. `{1,2,[4,5],3}`
b. `{1,2,4,5,3}`
c. `SyntaxError`
d. `TypeError`
<details>
<summary>answer</summary>
TypeError, because a set can store only immutable objects such as number (int, float, complex or bool), string or tuple
</details>

6. What will be the output?
```python
    my_set: set = {10,20,30,40,50}
    print(my_set[0:2]) 
```
a. `{10, 20}`
b. `{10, 20, 30}`
c. `IndexError`
d. `TypeError`
<details>
<summary>answer</summary>
TypeError, because sets are unordered, so indexing doesn't work
</details>

7. what will be the output?
```python    
    my_set: set = {1, 2, 3, 4, 5, 'A', 'a'}
    print(my_set.discard({1,2,3})) 
```
a. `{4, 5, 'A', 'a'}`
b. `{1, 2, 3}`
c. `None`
d. `KeyError`
<details>
<summary>answer</summary>
None, because discard() only removes a single element. {1, 2, 3} is a set itself, not an element within my_set. Therefore, discard does not find it and returns None.
</details>

8. what will be the output?
```  python 
   my_set: set = {1, 2, 3, 4, 5, 'A', 'a'}
   my_set.difference_update({1, 5, 3, 'A'})
   print(my_set)
 ```
a. `None`
b. `{2, 4, 'a'}`
c. `TypeError`
d. `{1, 5, 3, 'A'}`
<details>
<summary>answer</summary>
 {2, 4, 'a'} since difference_update() method is used to remove multiple element at once.
</details>

9. What's the difference betwee` discard()` and` remove()` method?
a.` discard() remove multiple items and remove() method is used to remove single item.`
b. `remove() raises error if the item is not found and discard() does not raise error.` 
c. `discard() raises error if the item is not found() and remove does not raise error.`
d. `both method raises error if the item is not found.`
<details>
<summary>answer</summary>
 b, because discard() does not raises error if the item is not found.
</details>

10. Hashable objects are?
a. `mutable`
b. `immutable`
c. `both a & b`
d. `None`
<details>
<summary>answer</summary>
 immutable, since only immutable objects are hashable.
</details>

11. What will be the output?
```python
     my_set: set = {1, 2, 3, 4, 5}
     my_set2 = my_set
     my_set.add(7)
     print(my_set is my_set2)
``` 
a. `SyntaxError`
b. `False`
c. `True`
d. `None`
<details>
<summary>answer</summary>
 True, they’re the same object, In mutable types (lists, sets, dicts), methods mutate the one shared object → all references observe the change.
</details>

12.  What will be the output?
```python
     Set = {1,2,3}
     print(hash(Set))
```
a. `This will print a hash value (an integer)`
b. `SyntaxError`
c. `KeyError`
d. `TypeError`
<details>
<summary>answer</summary>
 TypeError, because sets are mutable hence it is unhashable
</details>

13.    What will be the output?
```python
      my_set:  set = {1,2,3, "Hello! World", 4,5,6}
      my_set2: set = {1,2,3, "Hello! World", 8,9}
      print(my_set.symmetric_difference(my_set2))
```
a. `Return a set containing the difference between two sets`
b. `Return a set that contains all items from both sets, duplicates are excluded`
c. `Return a set that contains only unique items from both sets`
d. `None of them`
<details>
<summary>answer</summary>
 c, it return a set that contains only unique items from both sets
</details>

14. What will be the output?
```python
     Set = {2,3,5,6,7}
     Set2 = Set.copy()
     print(Set is Set2) 
```
a. `True`
b. `False`
c. `TypeError`
d. `None of them`
<details>
<summary>answer</summary>
 False because Set.copy() creates a shallow copy of the set. Set1 and Set2 are not the same object in memory, even though their contents are equal.
</details>

15.  What will be the output?
```python
     frozen_set1: frozenset = frozenset([1, 2, 3, 4])
     copy_set: frozenset = frozen_set1.copy()
     print(frozen_set1 is copy_set)
```
a. `True`
b. `False`
c. `TypeError`
d. `None of them`
<details>
<summary>answer</summary>
 True, because frozensets are immutable so it just returns a reference to the same object. 
</details>

16.  When an object's reference count reaches 0, means it is no longer needed then what will     happen to it?
a. `it will always remain in memory`
b. `The garbage collector free up memory occupied by these objects.`
c. `The object is converted to None automatically`
d. `Python raises an error immediately`
<details>
<summary>answer</summary>
 b, The garbage collector free up memory occupied by these objects.
</details>

17.  What will be the output?
```python
     s = {True, 1, 2}
      print(len(s))
```
a. `3`
b. `2` 
c. `1`
d. `TypeError`
<details>
<summary>answer</summary>
 2, because In Python, True is equal to 1, so {True, 1} collapses to a single item in a set. Thus, the set becomes {1, 2} and has length 2.
</details>

18.   What will be the output?
```python
     s = {1, 2, 3}
     s.update([4], (5,), {6})
     print(s)
```
a. `{1, 2, 3, 4, 5, 6} `
b. `{1, 2, 3, [4], (5,), {6}}`
c. `TypeError`
d. `{1, 2, 3}`
<details>
<summary>answer</summary>
 a, The update() method can take any iterable. All values from lists, tuples, and other sets are unpacked and added to s.
</details>

19.  What will be the output?
```python
     a = set("hello")
     b = set("world")
     print(a & b)
```
a. `{'l', 'o'} `
b. `{'h', 'e', 'l', 'o', 'w', 'r', 'd'}`
c. `set()`
d. `TypeError`
<details>
<summary>answer</summary>
 a, a & b computes the intersection of two sets, which includes characters common to both strings.
</details>

20.  What will be the output?
```python
     print({frozenset({1, 2}), frozenset({2, 1})})
```
a. `{frozenset({1, 2}), frozenset({2, 1})}`
b. `{frozenset({1, 2})} `
c. `TypeError`
d. `None of the above`
<details>
<summary>answer</summary>
 b, frozenset({1, 2}) and frozenset({2, 1}) are equal (order doesn't matter), so only one is kept in the set.
</details>


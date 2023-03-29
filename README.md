# python-assignment-4
# Python Basic Assignment
## Assignment - 4
-------------------------
### 1. What exactly is []?
[] is the empty list.

### 2. In a list of values stored in a variable called spam, how would you assign the value 'hello' as the third value? (Assume [2, 4, 6, 8, 10] are in spam.)
In order to assignn 'hello' at 3rd value. We need to modify the value at index 2 of spam list
spam = [2, 4, 6, 8, 10]
print(spam)
spam[2] = 'hello'
print(spam)

## Let's pretend the spam includes the list ['a', 'b', 'c', 'd'] for the next three queries.
spam = ['a', 'b', 'c', 'd']
### 3. What is the value of spam[int(int('3' * 2) / 11)]?
- '3'**2 will give '33'
- int('33') will be 33
- 33/11 will be 3.0
- int(3.0) will give 3
- spam[3] will be value at index 3 that is 'd'
spam[int(int('3'*2)/11)]

### 4. What is the value of spam[-1]?
- spam[-1] = last value of list that is 'd'
spam[-1]

### 5. What is the value of spam[:2]?
- spam[:2] = 'a' and 'b'
spam[:2]

## Let's pretend bacon has the list [3.14, 'cat,' 11, 'cat,' True] for the next three questions.

bacon = [3.14, 'cat', 11, 'cat', True]
### 6. What is the value of bacon.index('cat')?
- It will output the index of first occurence of 'cat' value
- ans: 1
bacon.index('cat')
### 7. How does bacon.append(99) change the look of the list value in bacon?
- It will append 99 at the end of list bacon
- [3.14, 'cat', 11, 'cat', True, 99]
bacon.append(99)
print(bacon)
### 8. How does bacon.remove('cat') change the look of the list in bacon?
- It will remove the first occurence of the 'cat'
- [3.14, 11, 'cat', True, 99]
bacon.remove('cat')
print(bacon)

### 9. What are the list concatenation and list replication operators?

- List concatenation operator is ‘+’ while list replication operator is ‘*’

### 10. What is difference between the list methods append() and insert()?
- Append method appends the given object to the end of the list always.
- Insert method accepts two arguments, index at which the element needs to be inserted and the object to insert.

### 11. What are the two methods for removing items from a list?
Two methods used for removing items from a list are:
- List.remove(object) -> Removes the first occurrence of the given object from the list
- List.pop(index = -1) -> Removes and returns item at the index (default is -1, the last element)

### 12. Describe how list values and string values are identical.

While list is a collection of values in Python, string is a collection of characters. Both list and strings are iterable in Python and a for loop can be used around a list or string object to iterate through each element in the list/string.

### 13. What's the difference between tuples and lists?
Tuples are immutable where as lists in Python are mutable. So once created, the items inside a tuple cannot be changed.

### 14. How do you type a tuple value that only contains the integer 42?
tup = tuple([32])
tup = tuple([32])
print(tup)

### 15. How do you get a list value's tuple form? How do you get a tuple value's list form?
By using type casting
1. b = tuple([42, 3, 5])
2. type(b)  # tuple
3. c = list(b)
4. type(c) # list
b = tuple([42, 3, 5])
type(b)  # tuple
c = list(b)
type(c) # list

### 16. Variables that "contain" list values are not necessarily lists themselves. Instead, what do they contain?
They contain references to the list values
var = [1,2,3]
print(var)
print(id(var))

### 17. How do you distinguish between copy.copy() and copy.deepcopy()?
- copy() returns a shallow copy of list and deepcopy() return a deep copy of list.
- deepcopy: In case of deep copy, a copy of object is copied in other object. It means that any changes made to a copy of object do not reflect in the original object.
- shallow copy: In case of shallow copy, a reference of object is copied in other object. It means that any changes made to a copy of object do reflect in the original object.

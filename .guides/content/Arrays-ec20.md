Variables store one item of data but arrays, which are similar, can store multiple items of data.

An array can store multiple items of data called elements under the same identifier.
The definition usually states that the elements must be of the same data type but in some programming languages such as JavaScript and Python different data types can be stored in the same array.

An array can be created by specifying the elements stored in it. This is called **declaring** the array.
Here are two arrays:
```
array friends = [“Catherine”, “Stephen”, “Jack”, “Rosie”, “Matthew”]
array ages = [17, 14, 9, 9, 15]
```
Each element in an array has an index position (just as the characters in a string).
![](.guides/img/array.png)
Like a string, the length of an array can be found and it can be traversed, added to and split into sub-arrays.
```
for index = 0 to friends.length – 1
if friends[index] == “Jack” then
  position = index
endif
print(index)
```

The print statement would return the number 2.

The elements in the array can be edited. The following would change name.
```
for index = 0 to friends.length – 1
if friends[index] == “Jack” then
  friends[index] = “David”
endif
```


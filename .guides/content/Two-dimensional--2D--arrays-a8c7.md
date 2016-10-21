A multidimensional array is an array of arrays and in a two dimensional array there is a second array at each index position of the 1D array.

A 2D array can be represented by a **matrix**.

For example a student may have recorded the temperature in the morning, at noon and in the evening, every day for a week.
The temperatures could be recorded in the following matrix:

![](.guides/img/2darray.png)

The days of the week are represented by the rows 0 to 7 and the temperature recordings by the columns 0 to 2.

The array would be declared as:
```array temperatures [7, 3]```

**To assign values to the array**

```
temperatures[0, 0] = 10
temperatures[0, 1] = 15
temperatures[0, 2] = 9
temperatures[1, 0] = 11 etc.
```

This could be done using loops.

**Printing data**
```
print(temperatures[3, 1] //would return the number 9.

print(temperatures[6, 2] //would return the number 11.
```

**The student could write an algorithm to find the average temperature for each day:**
```
for index = 0 to temperatures.length – 1 //The loop will run from 0 to 6.
total = 0  //’total’ and ‘average’ are set to 0 for each turn of the loop.
average = 0
for element = 0 to 2  //The three items at each index are added together.
    total = total + temperatures[index, element]
  next element
  average = total / 3
  print(average)
next index
```
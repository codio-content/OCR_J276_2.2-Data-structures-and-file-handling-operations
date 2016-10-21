Data stored in programs can be saved to text files on secondary storage devices so they are not lost when the computer is switched off. They can then be loaded back into the program.

Saving the data to a text file is called ‘writing’ and loading it back in is called ‘reading’.

### Writing
Before a file can be accessed or opened, it must be given a fi le handle. A file handle is a reference assigned to the file so that the program can access it.

In OCR pseudocode this is done using the following command:
```
myFile = openWrite(“sample.txt”)
```

When the writing has finished, the file must be closed:
```
myFile.close()
```

To save the names of friends in the array, the student could write the following code:
```
array friends = [“Catherine”, “Stephen”, “Jack”, “Rosie”, “Matthew”]
friendsFile = openWrite(“friends.txt”)
for index = 0 to friends.length – 1
  friendsFile.writeLine(friends[index])
next index
friendsFile.close()
```
Each name will be stored on a new line in the file.

### Reading
The data can be read from a text file using the following command;
```
myFile = openRead(“sample.txt”)
```
To load the data back into the array, the student could use the following code:
```
friendsFile = openRead(“friends.txt”)
for index = 0 to 4
  friends[index] = friendsFile.readLine()
next index
friendsFile.close()
```
If you are not sure how many entries there are then **endOfFile** can be used:
```
friendsFile = openRead(“friends.txt”)
while NOT friendsFile.endOfFile()
  friends[index] = friendsFile.readLine()
endwhile
friendsFile.close()
```
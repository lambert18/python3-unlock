# python3-unlock
This is for public, anyone can copy the code. But make sure what you copy that you can understand.<br />
This code only shared when i got some real / study case (assignment from school / college).

## Make Pattern
The pict show:<br />
![Case 1](https://i.stack.imgur.com/qtOe4.png)

<p>Converting numbers (i.e. 10) to a string, then taking a substring starting at character zero and ending before character 1. This will always be '1',
converting that back to an int (i.e. 1).
Then comparing that to 10. Since 1 does not equal 10, all you're doing is printing number + 1 after your first print
Something similar would work if use range(numbers) instead, but without another loop it's still only going to print one more column</p>

You can use any solutions below:<br />

### Solution 1
```
numbers = 10

for number in range(numbers):
    for i in range(numbers):
        print (number,end="\t")
        number += 1
    print('\n',end='')
```

### Solution 2
```
numbers = 10
for number in range(numbers):
    rowString = ''
    for numIndex in range(numbers):
        rowString += str(numIndex + number) + '\t'
    print(rowString)
```

### Solution 3
```
numbers = 10
for number in range(numbers):
    print("\t".join([str(index) for index in range(number, numbers + number )]))
```

# python3-unlock
This is for public, anyone can copy the code. But make sure what you copy that you can understand.<br />
This code only shared when i got some real / study case (assignment from school / college).

## Make Pattern
The pict show:<br />

<div align="center">
<img src="https://i.stack.imgur.com/qtOe4.png" >
<p>Perfectly balanced</p>
</div>

<p>Converting numbers (i.e. 10) to a string, then taking a substring starting at character zero and ending before character 1. This will always be '1',
converting that back to an int (i.e. 1).
Then comparing that to 10. Since 1 does not equal 10, all you're doing is printing number + 1 after your first print
Something similar would work if use range(numbers) instead, but without another loop it's still only going to print one more column</p>

You can use any solutions below:<br />


### Solution 1
```python3
numbers = 10

for number in range(numbers):
    for i in range(numbers):
        print (number,end="\t")
        number += 1
    print('\n',end='')
```
#### Explanation
`numbers = 10` Defines Variable. But if you don't want that variable, you can input `for number in range(10):`
If you want input code without variable, the code should like:
```python3
for number in range(10):
    for i in range(10):
        print (number,end="\t")
        number += 1
    print('\n',end='')
```
<br />

`number += 1` is an operator used for every first number has been added 1 for each loop.
It's like 
```python3
print (number,end="\t")
number += 1
print (number,end="\t")
number += 1
print (number,end="\t")
number += 1
```
until 10 times.

<br />

The `end=` keyword argument dictates what should be printed after all of the arguments have been printed. <br />
the backslash `\` is a special character, also called the "escape" character. It is used in representing certain whitespace characters: <br />
`\t` is a tab <br />
`\n` is a newline <br />

---

### Solution 2
```python3
numbers = 10
for number in range(numbers):
    rowString = ''
    for numIndex in range(numbers):
        rowString += str(numIndex + number) + '\t'
    print(rowString)
```
#### Explanation
`numbers = 10` Defines Variable. But if you don't want that variable, you can input `for number in range(10):`
If you want input code without variable, the code should like:
```python3
for number in range(10):
    rowString = ''
    for numIndex in range(10):
        rowString += str(numIndex + number) + '\t'
    print(rowString)
```
<br />



---

### Solution 3
```python3
numbers = 10
for number in range(numbers):
    print("\t".join([str(index) for index in range(number, numbers + number )]))
```

---

## Create Decimals in 5 lines (Loop)
The pict show:<br />
![Case 1](https://i.stack.imgur.com/qtOe4.png)

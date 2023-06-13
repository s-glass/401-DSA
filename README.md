# 401 Python - Data Structures and Algorithms

---------------------------------
## Code Challenge: Class 01
Create a function that returns list elements in reverse order.

Created in a group with Dan Quinn, Anthony Sinista, Jared Ciccarello, Andrew Carroll, and Ashley Taylor

* Resources: Repl.it and Chat GPT

### Whiteboard Process

![Code Challenge 01](cc01-whiteboard.png)

### Approach & Efficiency

* Dan initially found this solution approach
* Big O include a time complexity of 0(n) and space complexity of 0(1)

### Solution

def reverse_list(list):

for i in range(len(list) // 2):
    temp = list[i]
    list[i] = list[len(list) - i -1]
    list[len(list) - i - 1] = temp

return list

list = [1,2,3,4]

reverse_list(list)
print(list)

---------------------------------

## Code Challenge: Class 02
Create a function called insertShiftArray which takes in an array and a value to be added. Without using built-in methods, return an array with the new value in the middle index.

Created in a group with Dan Quinn, Jared Ciccarello, and Ashley Taylor

* Resource: (https://stackoverflow.com/questions/48561673/adding-items-in-the-middle-of-a-list-in-python)

### Whiteboard Process

![Code Challenge 02](cc02-whiteboard.png)

### Approach & Efficiency

* This approach defines the list to be added to, creates a function that defines the list midpoint and adds the value to the middle, then simply prints the function.
* Regarding efficiency, this solution has a time complexity of O(n) since we are
* Big O include a time complexity of 0(n) and space complexity of 0(1).

### Solution

list = [ 3, 12, 17, 2, 8 ] # these are random list numbers

def insertShiftArray
    midpoint = len(list) // 2
    shiftArray = list[0:midpoint] + [value to be added] + list[midpoint:]

print insertShiftArray => [ 3, 12, 17, value to be added, 2, 8 ]


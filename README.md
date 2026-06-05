# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
```
import math

class cse:
    def mech(self, r):
        area = math.pi * r * r
        print("Area of the circle:", area)

radius = float(input("Enter the radius of the circle: "))
obj = cse()
obj.mech(radius)

```

## Output
<img width="472" height="217" alt="Screenshot 2026-06-05 203829" src="https://github.com/user-attachments/assets/79276e49-1769-444a-9faa-5aefea4ac351" />

## Result
Thus, the program has been excecuted successfully.


# Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
```
def merge(dict1, dict2):
    merged = {**dict1, **dict2}
    return merged

dict1 = {'a': 1, 'b': 2, 'c': 3}
dict2 = {'d': 4, 'e': 5, 'b': 10}

result = merge(dict1, dict2)
print("Merged dictionary:", result)
```
## Output
<img width="712" height="197" alt="Screenshot 2026-06-05 203928" src="https://github.com/user-attachments/assets/1d227503-afa8-48fe-aa61-f36c29e680d8" />

## Result
Thus, the program has been excecuted successfully.


# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

## 🧪Program
```
data = {'banana': 'yellow', 'apple': 'red', 'cherry': 'pink', 'grape': 'purple'}
sorted_by_keys = dict(sorted(data.items()))
sorted_by_values = dict(sorted(data.items(), key=lambda item: item[1]))
print("Original dictionary:", data)
print("Sorted by keys:", sorted_by_keys)
print("Sorted by values:", sorted_by_values)
```
## Sample Output
<img width="925" height="298" alt="Screenshot 2026-06-05 204020" src="https://github.com/user-attachments/assets/f63a0beb-2c36-4cef-a65e-baa3d5136002" />

## Result
Thus, the program has been excecuted successfully.


# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
```
list1 = [10, 20, 30, 40]

try:
    print(list1[5])
except IndexError:
    print("You're out of list range")
```
## Output
<img width="411" height="198" alt="Screenshot 2026-06-05 204109" src="https://github.com/user-attachments/assets/3cc5d9e5-e029-4c50-9179-ef815b5833e2" />

## Result
Thus, the program has been excecuted successfully.


# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
def count_lines(filename):
count = 0
with open(filename, "r") as file: 
    for line in file:
        if not line.startswith('T'):
            count += 1
result=count_lines("story.txt")
print("Number of lines not starting with 'T':", result)
```
## Output
<img width="516" height="183" alt="Screenshot 2026-06-05 213938" src="https://github.com/user-attachments/assets/12e248b5-5870-46bd-b46a-4c17e393491b" />

## Result
Thus, the program has been excecuted successfully.

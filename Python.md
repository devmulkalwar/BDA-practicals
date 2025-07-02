## Practical 1: Create a list and perform the following methods

## Code:
```py
# Create a list
fruits = ["apple", "banana", "cherry", "date"]
print("Original list:", fruits)

# Append
fruits.append("elderberry")
print("After append:", fruits)

# Insert
fruits.insert(2, "blueberry")
print("After insert at index 2:", fruits)

# Remove
fruits.remove("banana")
print("After remove 'banana':", fruits)

# Pop
popped = fruits.pop()
print("Popped item:", popped)
print("After pop:", fruits)

# Sort
fruits.sort()
print("After sort:", fruits)

# Reverse
fruits.reverse()
print("After reverse:", fruits)

# Index
index = fruits.index("cherry")
print("Index of 'cherry':", index)

# Count
count = fruits.count("apple")
print("Count of 'apple':", count)

# Extend
more_fruits = ["fig", "grape"]
fruits.extend(more_fruits)
print("After extend:", fruits)

# Clear
fruits.clear()
print("After clear:", fruits)
```
# Bubble Sort
## General Idea
```
# Bubble Sort Algorithm 
for i in range(len(lst)): # Loop over the whole list  
    for j in range(len(lst) - 1): # Check the next element in the list
        if lst[j] > lst[j + 1]:
            # swap elements
            lst[j], lst[j + 1] = lst[j + 1], lst[j]
```
## Bubble Sort Function
```
def bubble_sort(lst):
 
    # outer loop to access each list element
    for i in range(len(lst)):
 
        # inner loop to compare list elements
        for j in range(len(lst) - 1):
 
            # swap elements if necessary
            if lst[j] > lst[j + 1]:
                lst[j], lst[j + 1] = lst[j + 1], lst[j]
 
    return lst       
 
data_list = [15, 16, 6, 8, 5]
print(f"Unsorted List: {data_list}")
 
sorted_list = bubble_sort(data_list)
 
print(f"Sorted List: {sorted_list}")
```
## Bubble Sort in Descending Order
```
def bubble_sort(lst):
    # outer loop to access each list element
    for i in range(len(lst)):
 
        # inner loop to compare list elements
        for j in range(len(lst) - 1):
 
            # swap elements if necessary
            if lst[j] < lst[j + 1]:
                lst[j], lst[j + 1] = lst[j + 1], lst[j]
 
    return lst


# take integer inputs and convert it to a list    
data_list = list(map(int, input().split()))

sorted_list = bubble_sort(data_list)
print(sorted_list)
```
## Optimized Bubble Sort
```
# Bubble sort in ascending order
def bubble_sort(data):
 
    for i in range(len(data) - 1):
        swapped = False
        for j in range(len(data) - 1 - i):
            if data[j] > data[j + 1]:
                data[j], data[j+1] = data[j+1], data[j]
                swapped = True
        if not swapped:
            break
        
    return data
 
data_list = [4, 6, 99, 45, 0]
 
sorted_list = bubble_sort(data_list)
print(sorted_list)
```
## Descending Optimized Bubble Sort
```
def bubble_sort(lst):
    # Bubble sort in descending order
 
    for i in range(len(lst) - 1):
        swapped = False
        for j in range(len(lst) - 1 - i):
            if lst[j] < lst[j + 1]:
                lst[j], lst[j+1] = lst[j+1], lst[j]
                swapped = True
        if not swapped:
            break
        
    return lst 


# take integer inputs and convert it to a list
data_list = list(map(int, input().split()))

sorted_list = bubble_sort(data_list)
print(sorted_list)
```
## Time Complexity
The time complexity is based on the number of comparisons.
## Applications
Use Bubble Sort for
- Small data sets
- Simplicity over efficiency
- Data is already partially sorted

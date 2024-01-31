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

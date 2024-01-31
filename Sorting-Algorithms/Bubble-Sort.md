```
# Bubble Sort Algorithm 
for i in range(len(lst)):   
    for j in range(len(lst) - 1):   
        if lst[j] > lst[j + 1]:
            # swap elements
            lst[j], lst[j + 1] = lst[j + 1], lst[j]
```

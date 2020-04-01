# Guide to Big O Notation

**Definition:** 
How the runtime scales with respect to some input variables. 
An equation that expresses how the runtime scales or changes. 

## 4 Rules

1) Different steps added together (the amount of time it takes to get through all steps)
2) Drop constants 
    Example: A function that simultaneously runs an array through 2 loops.
            This may seem like it is O(2N) but we drop the the constant (the 2) 
            and just call it O(N) because it will take the same amount of time 
            to run through both loops
            O(2N) => O(N)
3) Different inputs require different variables
    2 nested loops (or operations) through 2 different arrays 
    O(N^2) => O(a * b)
4) Drop non-dominant terms
    If your function has one loop that is O(N) and another that is O(N^2) drop the O(N)
    because the second loop will always take longer when scaled and is therefore dominant
    O(N) + O(N^2) => O(N^2) 

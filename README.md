# C Contracts

A contract file in C is a specialized header file that simply defines that certain function/variables exist, but is not necessarily accompanied by an implementation.
For example:

list.x (contract files use a(n) .x extension)  
list1.o  
list2.o

Both list1.o and list2.o implement the functions defined in list.x.
During linking, EITHER list1.o or list2.o could be used.

## Benefits

### Improvements

If a current implementation is not performing well enough, a custom implementation can be made.
No other code would need to be altered during the transition.
Only a new implementation would need to be written.

### Standardization

Standards could be set for common data structures and algorithms.
This way, say a list from this vendor would be easily replacable by a list from this other vendor.

Aditionally, standards could be superceeded quite easily.
A new standard could define all the same features as the old, and more.
Old code would still work with the new standard, and new features could be used by the new code.

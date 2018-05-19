Tasfia Addrita
CISC 2200 - Homework 7

#### Problem 3

```
p = L // executed once
while p != NULL do
begin
	q = p // executed n times
	while q != NULL do // iterating where p is to the end of list; first time through outer while loop, executes n times; final loop will execute only once
	begin
		q = q -> next // executed n^2/2 times
		r = L // executed n^2/2 times
		while r != q do // iterating from beginning of list to where q is; when first outer executes, this loop executes once; last time outer loop executes, this loop executes 10 times
			r = r -> next
		end
		p = p -> next // executed n times
end
```

#### Problem 7

1. This addition will be easy to implement in the array-based SortedType because the item can easily be identified by its index. A single variable can be used to store the position of the last added element.
2. This addition will not be easy to implement for linked based lists because elements cannot be accessed randomly. When a new element is added, the position of the element stored in previous nodes also changes just to incorporate the sorted order.

#### Problem 8

1. This addition will not be easy to implement in the array-based SortedType. Because the list is sorted, removing an element of the array would require a shift in all of the remaining elements. 
2. This addition will be easy to implement in linked SortedType. The next pointer variable is set to null. Once the location is known, only the pointers need to be updated to remove an element, and the whole list does not be shifted like an array would. 

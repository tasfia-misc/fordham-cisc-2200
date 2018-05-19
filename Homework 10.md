Tasfia Addrita
CISC 2200 - Homework 10

#### Problem 2

A circular linked list has a last node that does not contain a NULL pointer. instead the last node contains a pointer that has the address of the first node and therefore points back to the first node creating a circular doubly linked list. The advantages of a doubly linked list include that the list can be traversed from both directions, meaning that you can go from the head to the tail of the list or from the tail to the head of the list. Another advantage is that jumping from head to tail or from tail to head is done so in constant time, or O(1). A disadvantage of the circular doubly linked list is that it takes a slightly larger amount of memory in each node to accommodate the previous pointers each time. Another disadvantage is that there can be a lot of pointers involved in the list, therefore extra caution has to be taken care of in handling otherwise data could be potentially lost.

#### Problem 3

|                       Contiguous List                        |                      Singly linked list                      |                      Doubly linked list                      |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|                       Is a fixed size                        | A node on a singly linked list cannot be removed unless we have the pointer to its predecessor | Insertion and deletion algorithms are more complicated compared to singly linked list |
| Need to know exact number of elements needed in array before you allocate it | A singly linked list can only be traversed in one direction  | Insertion and deletion take more time because more pointer operations are required than that of a singly linked list |
|  If you over allocate space – then you can be wasting space  | Cannot randomly access any element like you can in an array by index – have to transverse through all the nodes | Requires more space per node because one extra field is required for pointer to previous node |
| Adding and deleting elements into the array are therefore costly since your wasting time or wasting space |  Accessing time in array is O(1) but in linked list is O(n)  |                                                              |
|                                                              | Cannot transverse it from the end – only from the beginning  |                                                              |
|                                                              |      Not easy to sort elements in a singly linked list       |                                                              |

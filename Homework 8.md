Tasfia Addrita
CISC 2200 - Homework 8

#### Problem 3

In order to implement both stacks in one array, we can declare a class DoubleStack which has two top variables. One top variable is used for the stack of small values, and another top variable can be used for the stack of large values. The class should contain the Push() function to add elements, and two Pop() functions should be used—one for small values, and another for large values.



|  0   |  1   |  2   | ...  | 198  | 199  |
| :--: | :--: | :--: | :--: | :--: | :--: |
|      |      |      |      |      |      |

```c++
class DoubleStack {
    public:
	DoubleStack();
	void Push(int a);
	void PopSmall();
	void PopLarge();
	int topSmall;
	int topLarge;
    
    private:
    	int array[200];
};

```

```c++
void DoubleStack::Push(int a) {
    if (a <= 1000) {
        topSmall++;
        array[topSmall] = a;
    } 
    else {
	topLarge—;
	array[topSmall] = a;
    }
}

```

#### Problem 4

1. A stack can also be said to be, at a logical level, an ordered group of homogeneous items as arrays. However, the value at index position 0 has a different kind of significance compared to the other elements so this would be fine. 
2. This implementation would not change the stack specifications themselves but instead it would require changes to the implementation of the functions instead. 
3. The implementation of the function would change because there would need to be a shift in the elements when the element at the top of the stack is removed. If the stack elements are outputted with the first element first, then that would have to start from the end of the array up until index 0 because stacks are logically implemented with last in/first out. Therefoe, you would have to do the reverse to have the first in element to be outputted first too. This implementation would also disrupt the size of the array because lets say, if it has a size of 20 and a user only wants to add 10 elements, additional code would be necessary to take in the size of the input given by the user to accurately fit the number of elements since it is being added from the end and not from the beginning because of LIFO logic.

#### Problem 5

```c++
#include //header files
#include <string>
#include “StackType.h”

int main() {
	char c = str.at(i);
	int i = 0;
	StackType stack;
	string str;
	cout << “Enter a string” << endl;
	getline(cin,str);
	while (c != ‘.’) {
		stack.Push(c);
		c = str.at(i++);
	}
	bool palindrome = true;
	string::iterator iter;
	for(iter = str.begin(); palindrome && (stack.IsEmpty()); iter++) {
		palindrome = *iter = stack.Top();
		stack.Pop();
	}
	if (palindrome)
		cout << str << “is a palindrome” << endl;
	else
		cout << str << “is not a palindrome” << endl;
	
	return 0;
}
```

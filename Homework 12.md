Tasfia Addrita
CISC 2200 - Homework 12

#### Problem 4

1. ```c++
   int Sum(int info[], int fromIndex, int toIndex) { // computes the sum of the items between fromIndex and toIndex
       if (fromIndex == toIndex)
           return info[toIndex]
       else
           return fromIndex + sum(info, fromIndex + 1, toIndex);
   ```

2. recursive case: when fromIndex and toIndex are different
   base case: when fromIndex and toIndex are the same

3. Sum(number, 0, MAX_ITEMS - 1)

4. There can be a run time error due to negative indexes or due to fromIndex being greater than toIndex

#### Problem 5

1. There is no base condition
2. Does not involve recursion and it does not calculate the sum of the squares but just the sum
3. Nothing is wrong
4. Nothing is wrong
5. The logic is wrong in the general case

#### Problem 9

| call | info | fromlocation | tolocation | midpoint | result |
| :--: | :--: | :----------: | :--------: | :------: | :----: |
|  1   |  2   |      0       |     9      |    4     | false  |
|  2   |  2   |      5       |     9      |    7     | false  |
|  3   |  2   |      8       |     9      |    8     |  true  |


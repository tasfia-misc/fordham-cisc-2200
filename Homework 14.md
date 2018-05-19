Tasfia Addrita
CISC 2200 - Homework 14

#### Problem 1

1. For a binary tree the big O notation would be O(log2N) because the size of the structure that will be searched would be reduced when traversing through each subtree. This is because of the structure of the binary tree, which means that the left subtree contains value less than the root and the right subtree contains the values greater than the root.

   For a sorted linked list the big O notation for searching for an element would be O(N) because each node would need to be accessed.

2. If the elements are inserted in order then the big O notation for both structures would be O(N) because each node in the linked list and each leaf in the binary tree would need to be traversed through.

#### Problem 6

1. bool isBST( treeNode* node, int min, int max) //returns true if a BT is a BST

2. ```c++
   bool treeType::isBST(treeNode* node, int min, int max) {
   	//empty tree is BST
   	if(node == NULL)
           return true;
   	if (node -> info < min || node -> info > max)
   		return false;
   	//check subtrees recursively
   	return isBST (node -> left, min, node -> info-1) && isBST(node -> right, node -> info + 1, max);
   }
   
   ```

#### Problem 9

1. It would be interested in a new leaf node on the right subtree of node 5
2. 0
3. Inorder
4. Preorder

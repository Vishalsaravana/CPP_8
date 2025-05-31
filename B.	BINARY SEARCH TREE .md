# BINARY SEARCH TREE

## PROGRAM STATEMENT:

To write a C++ function to convert a binary tree into a binary search tree


![image](https://github.com/user-attachments/assets/248d2b18-90a7-48f2-ba52-c008e0459528)

## ALGORITHM:  

1.	Start the program.
2.	Define Function: Create a function convertBST that takes the root of the BST, an InOrderArray, and an index i as input.
3.	Traverse Left Subtree: Recursively call convertBST on the left child of the current node.
4.	Assign Data: Assign the value from InOrderArray[i] to the current node’s data, then increment i.
5.	Traverse Right Subtree: Recursively call convertBST on the right child of the current node.
6.	End the program.

## PROGRAM:
```
void convertBST(node*root,vector<int> InOrderArray,int& i)
{
if(root){
convertBST(root->left,InOrderArray,i); root->data = InOrderArray[i++]; convertBST(root->right,InOrderArray,i);
}


}
``` 
## OUTPUT :
![image](https://github.com/user-attachments/assets/bf488857-58c6-46d0-8b5b-7417825f3f20)

## RESULT:

Thus, the C++ program to convert a binary tree into a binary search tree is created successfully.


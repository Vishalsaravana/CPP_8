# TREE REPRESENTATION AND TRAVERSALS

## PROGRAM STATEMENT:

To write a C++ Function to perform Inorder traversal of the below given tree.


![image](https://github.com/user-attachments/assets/400b1461-bed0-4aa8-b0de-8e03926bcd0d)

## ALGORITHM:  

1.	Start the program.
2.	Define Node: Create a Node structure with data and next pointer.
3.	Push: Insert a new node at the rear of the queue by updating the rear pointer.
4.	Pop: Remove the front node and update the front pointer, checking for underflow.
5.	Display: Print the queue from front to rear by traversing through all nodes.
6.	Display Front/Rear: Print the data of the front and rear nodes.
7.	Main: Perform push(), pop(), and display() operations on the queue.
8.	End the program.

## PROGRAM:
```
voidtraverseInOrder(struct node *dis)
{

if(dis!=NULL){ traverseInOrder(dis->left); cout<<" "<<dis->data; traverseInOrder(dis->right);
}


}
 ```
## OUTPUT :
![image](https://github.com/user-attachments/assets/1bce7534-d58d-4341-a437-832e0a07687a)

## RESULT:

Thus, the C++ program to perform Inorder traversal of the below given tree is created successfully.


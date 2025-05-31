# AVL TREE

## PROGRAM STATEMENT:

To write a C++ code to perform LL & RR rotation in an AVL Tree while inserting elements.

## ALGORITHM:  

1.	Start the program.
2.	Insert Node: Define the function insert() to insert a new key in the AVL tree. If the tree is empty, create a new node with the given key.
3.	Normal BST Insertion: Traverse the tree recursively and insert the node at the appropriate position based on the comparison of the key with the current node's key.
4.	Update Height: After insertion, update the height of the ancestor node based on the maximum height between the left and right child.
5.	Check Balance Factor: Calculate the balance factor of the current node to check if it has become unbalanced. If unbalanced, handle it with appropriate rotations (left or right).
6.	End the program.

## PROGRAM:
```
Node* insert(Node* node, int key)
{
/* 1. Performthe normal BST insertion*/ if (node == NULL)
return(newNode(key));

if (key< node->key)
node->left = insert(node->left, key); else if (key> node->key)
node->right =insert(node->right, key); else // Equalkeys are not allowed in BST
returnnode;

/* 2. Update height of this ancestor node */ node->height = 1 + max(height(node->left),
height(node->right));

/* 3. Get thebalance factor ofthis ancestor
node to checkwhetherthisnodebecame unbalanced */
int balance=getBalance(node);

// Ifthis nodebecomesunbalanced, then
 
// thereare 4 cases

// Left Left Case
if(balance > 1 && key< node->left->key) returnrightRotate(node);

// Right Right Case
if(balance <-1 && key> node->right->key) returnleftRotate(node);

// Left Right Case
if(balance > 1 &&key> node->left->key)
{
node->left = leftRotate(node->left); returnrightRotate(node);
}

// Right Left Case
if (balance < -1 && key< node->right->key)
{
node->right =rightRotate(node->right); returnleftRotate(node);
}

/* returnthe(unchanged) nodepointer*/ returnnode;
}
 ```
## OUTPUT :
![image](https://github.com/user-attachments/assets/64c973c4-70ed-47c8-9785-e8dbd336b801)

## RESULT:

Thus, the C++ program to perform LL & RR rotation in an AVL Tree while inserting elements is created successfully.



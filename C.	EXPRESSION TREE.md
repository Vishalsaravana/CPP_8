# EXPRESSION TREE

## PROGRAM STATEMENT:

To construct an expression tree from the given postfix expression. Generate the inorder and preorder traversal of the given expression tree below

![image](https://github.com/user-attachments/assets/6b736538-b0a8-4fd3-8868-7f0dad6552c5)

## ALGORITHM:  

1.	Start the program.
2.	Define Node Class: Create a node class with attributes value, left, right, and next. Initialize the node with a constructor to set value and set left and right to NULL.
3.	Constructor: The parameterized constructor initializes the value and sets left and right pointers to NULL. The default constructor sets left and right pointers to NULL.
4.	Friend Classes: Declare stack and expression_tree as friend classes so they can access private members of the node class.
5.	End the program

## PROGRAM:
```
class node
{
public:
char value; node*left; node*right; node*next=NULL; node(char c)
{
this->value=c; left=NULL; right=NULL;
}
 
node()
{
left=NULL; right=NULL;
}
friend class stack;
friend class expression_tree;
};
```

## OUTPUT :
![image](https://github.com/user-attachments/assets/d63d7655-aee3-43d2-bc0f-6ef0a41278a2)

## RESULT:

Thus, the C++ program to Generate the inorder and preorder traversal of the given expression tree below is created successfully.



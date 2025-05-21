# Ex23 Depth First Graph
## DATE: 21-05-2025
## AIM:
To compose the code for the function createNode to traverse the graph below in the depth first fashion.

![image](https://github.com/user-attachments/assets/63552824-d0a3-49c6-a473-6db27d1f03e4)

## Algorithm
1. Start
2. Allocate memory for a new node
3. Set the destination vertex value in the node
4. Set the node’s next pointer to NULL  
5. Return the new node  

## Program:
```
/*
Program to traverse the graph below in the depth first fashion
Developed by: Divya R V
RegisterNumber: 212223100005 
*/
```
```
struct node* createNode(int v) 
{
    struct node* newNode=malloc(sizeof(struct node));
    newNode->vertex=v;
    newNode->next=NULL;
    return newNode;
}

```
## Output:

![image](https://github.com/user-attachments/assets/95c3b60a-4a85-4023-818b-b1d1be7ae0eb)


## Result:
Thus, the C code for the function createNode to traverse the graph below in the depth first fashion is implemented successfully

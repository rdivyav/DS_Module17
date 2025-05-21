# Ex25 Adjacency List Representation
## DATE: 21-05-2025
## AIM:
To write a C program to represent the given graph using the adjacency list.

## Algorithm
1. Input Graph Details
2. Initialize Adjacency List
3. Define Node Structure
4. Insert Edges  
5. Display the Graph   

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: Divya R V
RegisterNumber: 212223100005 
*/
```
```
void printGraph(struct Graph* graph)
{
  int v;
  for(v=0;v<graph->numVertices;v++)
  {
      struct node *temp=graph->adjLists[v];
      printf("Vertex %d: ",v);
      while(temp)
      {
          printf("-> %d ",temp->vertex);
          temp=temp->next;
      }
      printf("\n");
  }
}
```
## Output:

![image](https://github.com/user-attachments/assets/08571580-6d57-417f-944d-ee31c2259644)


## Result:
Thus, the C program to represent the given graph using the adjacency list is implemented successfully

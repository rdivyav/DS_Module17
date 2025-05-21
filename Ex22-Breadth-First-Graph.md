# Ex22 Breadth First Graph
## DATE: 21-05-2025
## AIM:
To write a printQueue C function of the given graph that is to be traversed in the breadth first manner.

![image](https://github.com/user-attachments/assets/f483f48c-6af0-4027-a993-01c108a50933)


## Algorithm
1. Input number of vertices V and edges E
2. Create an adjacency matrix or list and initialize it 
3. Create a queue to hold vertices to visit
4. Create a visited array to keep track of visited vertices 
5. Enqueue the starting vertex, mark it as visited  

## Program:
```
/*
Program to traverse graph using BFS
Developed by: Divya R V
RegisterNumber: 212223100005 
*/
```
```
void printQueue(struct queue* q)
{
    int i=q->front;
    if(isEmpty(q))
     printf("Queue is empty");
    else
    {
        printf("Queue contains ");
        for(i=q->front;i<q->rear+1;i++)
         printf("%d ",q->items[i]);
    }
}
```
## Output:

![image](https://github.com/user-attachments/assets/feb58cdf-0b70-41c9-be01-a63c96764e46)


## Result:
Thus, the code for the printQueue function of the following graph that is to be traversed in the breadth first manner is implemented successfully.

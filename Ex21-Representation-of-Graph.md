# Ex21 Representation of Graph
## DATE: 21-05-2025
## AIM:
To write a C program to display the adjacency matrix of the given graph by supplying the edges and the number of vertices.

## Algorithm
1. Input number of vertices V and number of edges E  
2. Create a V x V adjacency matrix and initialize all elements to 0
3. Read the two vertices u and v that form an edge
Set adj[u][v] = 1

4.If the graph is undirected, also set adj[v][u] = 1 
5.Display the adjacency matrix   

## Program:
```
/*
Program to display the adjacency matrix of the given graph
Developed by: Divya R V 
RegisterNumber: 212223100005 
*/
```
```
int main()
{  int e1,e2,me,n,i;
    scanf("%d",&V);
    int adjMatrix[V][V];
    init(adjMatrix);
    n=V;
    me=n*(n-1);
    for(i=1;i<me;i++)
    {
        scanf("%d%d",&e1,&e2);
        addEdge(adjMatrix,e1,e2);
        if((e1==-1)&&(e2==-1))
         break;
    }
    printAdjMatrix(adjMatrix);
    return 0;
}
```
## Output:

![image](https://github.com/user-attachments/assets/60221bec-86b6-4133-9d0d-1806ede039ba)


## Result:
Thus, the C program to print the adjacency matrix of the given graph is implemented successfully.

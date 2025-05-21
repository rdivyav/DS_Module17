# Ex24 Topological Sort
## DATE: 21-05-2025
## AIM:
To compose the code to determine whether the topological ordering for the following graph is possible or not.

![image](https://github.com/user-attachments/assets/c74a7111-9b59-475c-aad4-9baf23d50ec0)


## Algorithm
1. Start 
2. Input number of vertices V and edges E 
3. Create an adjacency list for the directed graph
4. Initialize visited arrays 
5. For every vertex v from 0 to V-1:
6. In isCyclicDFS(v)
7. If any call detects a cycle → topological ordering not possible
8.  Else → topological ordering is possible
9.  Stop  

## Program:
```
/*
Program to determine whether the topological ordering for the following graph is possible or not
Developed by: Divya R V 
RegisterNumber: 212223100005 
*/
```
```
int main()
{
        int i,v,count,topo_order[MAX],indeg[MAX];

        create_graph();

        /*Find the indegree of each vertex*/
        for(i=0;i<n;i++)
        {
                indeg[i] = indegree(i);
                if( indeg[i] == 0 )
                        insert_queue(i);
        }

        count = 0;

        while(  !isEmpty_queue( ) && count < n )
        {
                v = delete_queue();
        topo_order[++count] = v; /*Add vertex v to topo_order array*/
                /*Delete all edges going from vertex v */
                for(i=0; i<n; i++)
                {
                        if(adj[v][i] == 1)
                        {
                                adj[v][i] = 0;
                                indeg[i] = indeg[i]-1;
                                if(indeg[i] == 0)
                                        insert_queue(i);
                        }
                }
        }

        //type your code here...
        if(count<n)
        {
            printf("No topological ordering possible, graph contains cycle\n");
            exit(1);
        }
        printf("Vertices in the topological order are :\n");
        for(i=1;i<=count;i++)
        {
            printf("%d ",topo_order[i]);
        }
        printf("\n");
        return 0;
}

```
## Output:

![image](https://github.com/user-attachments/assets/a4a94882-1d73-4b5e-8b72-f19e77e1baa0)

## Result:
Thus, the C program for determining whether the topological ordering for the following graph is possible or not, is implemented successfully.

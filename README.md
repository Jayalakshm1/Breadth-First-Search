LabExperiment1: Breadth First Search

Write a Python program to implement breath First Search. 

```Program:

graph = {
  '2': ['3', '4'],
  '3': ['5'],
  '4': ['6', '7'],
  '6': [],
  '5': ['6'],
  '7': ['8'],
  '8': []
}

visited = []  # List for visited nodes.
queue = []    # Initialize a queue

def bfs(visited, graph, node):  # Function for BFS
    visited.append(node)
    queue.append(node)

    while queue:  # Creating loop to visit each node
        m = queue.pop(0)
        print(m, end=" ")

        for neighbour in graph[m]:
            if neighbour not in visited:
                visited.append(neighbour)
                queue.append(neighbour)

# Driver Code
print("BFS order is")
bfs(visited, graph, '2')
```

Output:

![image](https://github.com/Jayalakshm1/Breadth-First-Search/assets/130430542/d6c52699-e71c-4910-86dc-0c39fde19b00)


Result:

Thus,Python program to implement breath First Search was executed successfully.

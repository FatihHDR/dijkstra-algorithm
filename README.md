# Implementation of Dijkstra's Algorithm in Python

Dijkstra's algorithm is a greedy algorithm used to find the shortest path from one source node to all other nodes in a weighted graph. Graphs can be directed or undirected, cyclic or acyclic, but the weights on all edges must be nonnegative.

## Steps:

### 1. Initialization:
- Create a set sptSet to track the nodes that are included in the shortest path tree. Start with an empty set.
- Set distance to all vertices as INFINITE. The source node distance is set to 0.

### 2. Iteration:

- As long as sptSet does not cover all nodes:
   - Select a node u that is not in the sptSet and has a minimum distance.
   - Add u to sptSet.
   - Update distance of all vertices adjacent to u:
     - For each vertex v adjacent to u, if distance(u) + weight(u, v) < distance(v), then update distance(v) to distance(u) + weight(u, v).

## illustration:
![image](https://user-images.githubusercontent.com/22562694/120260452-8d455d80-c2b3-11eb-9d84-6b8b46dffc2c.png)

The image above shows an example of Dijkstra's algorithm in action.
- `a` is the source node.
- Distances to all other nodes from the source are labeled positive infinity.
- Side weights are marked in light green.

## Output:
```
The shortest distance of  a  from the source vertex a is: 0
The shortest distance of  b  from the source vertex a is: 3
The shortest distance of  c  from the source vertex a is: 3.5
The shortest distance of  d  from the source vertex a is: 4.5
```

## Conclusion:
Dijkstra's algorithm is a powerful tool for finding the shortest path in a weighted graph. The algorithm is efficient and easy to implement. This algorithm has many applications in various fields such as navigation systems, network routing, and data analysis.

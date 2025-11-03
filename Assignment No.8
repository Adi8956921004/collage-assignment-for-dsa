from collections import deque

# ----------------------------
# Get user input for nodes and edges
# ----------------------------
num_locations = int(input("Enter the number of locations: "))

nodes = []
print("Enter the names of the locations:")
for _ in range(num_locations):
    name = input().strip()
    nodes.append(name)

# Mapping for node name <-> index
node_index = {node: idx for idx, node in enumerate(nodes)}

# Initialize empty adjacency list and adjacency matrix
adj_list = {node: [] for node in nodes}
adj_matrix = [[0]*num_locations for _ in range(num_locations)]

# ----------------------------
# Get edges (connections) from user
# ----------------------------
num_edges = int(input("Enter the number of direct connections (edges): "))
print("Enter each connection in the format: Location1 Location2")

for _ in range(num_edges):
    u, v = input().strip().split()
    # For adjacency list
    adj_list[u].append(v)
    adj_list[v].append(u)  # Since the graph is undirected

    # For adjacency matrix
    i, j = node_index[u], node_index[v]
    adj_matrix[i][j] = 1
    adj_matrix[j][i] = 1  # Undirected

# ----------------------------
# BFS using adjacency list
# ----------------------------
def bfs(graph, start):
    visited = set()
    queue = deque([start])
    order = []

    while queue:
        node = queue.popleft()
        if node not in visited:
            visited.add(node)
            order.append(node)
            queue.extend(neigh for neigh in graph[node] if neigh not in visited)
    
    return order

# ----------------------------
# DFS using adjacency matrix
# ----------------------------
def dfs(matrix, start_idx, visited=None, order=None):
    if visited is None:
        visited = set()
    if order is None:
        order = []

    visited.add(start_idx)
    order.append(nodes[start_idx])

    for i, connected in enumerate(matrix[start_idx]):
        if connected == 1 and i not in visited:
            dfs(matrix, i, visited, order)
    
    return order

# ----------------------------
# Get start node from user
# ----------------------------
start_node = input("Enter the starting location: ").strip()
start_index = node_index[start_node]

# ----------------------------
# Run BFS and DFS
# ----------------------------
bfs_result = bfs(adj_list, start_node)
dfs_result = dfs(adj_matrix, start_index)

# ----------------------------
# Print the results
# ----------------------------
print("\n--- Traversal Results ---")
print("BFS Traversal Order (Adjacency List):", ' → '.join(bfs_result))
print("DFS Traversal Order (Adjacency Matrix):", ' → '.join(dfs_result))

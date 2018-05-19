#In depth-first search, edges are explored
out of the most recently discovered vertex v that still has unexplored edges leaving
it. When all of v’s edges have been explored, the search “backtracks” to explore
edges leaving the vertex from which v was discovered. This process continues until
we have discovered all the vertices that are reachable from the original source
vertex. **If any undiscovered vertices remain, then one of them is selected as a new
source and the search is repeated from that source**. This entire process is repeated
until all vertices are discovered.

Unlike breadth-first search,
whose predecessor subgraph forms a tree, the predecessor subgraph produced by
a depth-first search may be composed of several trees, because the search may be
repeated from multiple sources.
In depth-first search, edges are explored
out of the most recently discovered vertex v that still has unexplored edges leaving
it. When all of v’s edges have been explored, the search “backtracks” to explore
edges leaving the vertex from which v was discovered. This process continues until
we have discovered all the vertices that are reachable from the original source
vertex. **If any undiscovered vertices remain, then one of them is selected as a new
source and the search is repeated from that source**. This entire process is repeated
until all vertices are discovered.

**Unlike breadth-first search,
whose predecessor subgraph forms a tree, the predecessor subgraph produced by
a depth-first search may be composed of several trees, because the search may be
repeated from multiple sources**.


**It may seem arbitrary that breadth-first search is limited to only one source whereas depth-first
search may search from multiple sources. Although conceptually, breadth-first search could proceed
from multiple sources and depth-first search could be limited to one source, our approach reflects
how the results of these searches are typically used. Breadth-first search is usually employed to find
shortest-path distances (and the associated predecessor subgraph) from a given source. Depth-first
search is often a subroutine in another algorithm.**


*Besides creating a depth-first forest, depth-first search also timestamps each vertex.
Each vertex v has two timestamps: the first timestamp d[v] records when v
is first discovered (and grayed), and the second timestamp f [v] records when the
search finishes examining v’s adjacency list (and blackens v).*

**The vertex from which we start gets blackened last (in all the edges that can be visited from it)
In BFS the vertex from which we start gets blackened first.**

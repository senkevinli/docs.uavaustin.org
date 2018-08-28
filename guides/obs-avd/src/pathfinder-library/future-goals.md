# Future Goals
Currently, alternate algorithms cannot be chosen easily.  Therefore, there is plan for restructuring pathfinder to be more modular such that different algorithms can be chosen at run time.  Moreover, with the insight that the shortest path always border on obstacles and the fact that all obstacles are circular, we can take advantage of this and make each obstacle a node in the graph, and generate weighted edges between them based on line of sight and distance.  This approach would completely eliminate the need to convert to a grid-based graph.
# Process pseudocode

## Process pixel map to graph of nodes
- Get region list using np.unique
- Initialize connection graph as N x N boolean diagonal matrix
- Find region edges by element n != element n+1 for each dimension
- for each region edge in each dimension, get associated regions from original map and set connection in graph to true

## Solve node puzzle
- Research solutions to graph coloring puzzle. I suspect there will be optimal solutions using linear algebra on connection matrix

## Return
- Give back the original image colored via an inputted color scheme or (default) as array of integers that can be mapped to colors later.
- Option to retireve node list and connection graph
- Option to retrieve region boundaries, n-dimensional or single dimension
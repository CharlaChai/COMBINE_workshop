# COMBINE_workshop
* [Step 1: Construct Cellular Graphs](#step-1-construct-cellular-graphs)
* [Step 2: Construct `CellularGraphDataset`](#step-2-construct-cellulargraphdataset)
* [Step 3 Initialise a Graph Neural Network (GNN)](#step-3-initialise-a-graph-neural-network-gnn)
* [Step 4 Train the GNN](#step-4-train-the-gnn)
* [Step 5 Evaluate the GNN](#step-5-evaluate-the-gnn)

# Step 1: Construct Cellular Graphs

We first construct cellular graphs as `networkx.Graph` using raw inputs including cell coordinates, cell types, biomarker expression, etc.

### A networkx.graph can be constructed using the inputs above

The function `spacegm.construct_graph_for_region` also generates some visualisations for each region, stored under `graph_img_output` and `voronoi_polygon_img_output`.

The full cellular graph for each region in the dataset can be accessed using the class method `get_full`:

And the n-hop (n=3 in this example) subgraph of region `i` around its center node `j` can be accessed using the class method `get_subgraph`: 

# Step 2: Construct `CellularGraphDataset`

`CellularGraphDataset` will be the major data container used in model training and evaluation. This object also handles all the featurization, subgraph sampling, and other necessary functionalities for SPACE-GM.

# Step 3: Initialise a Graph Neural Network (GNN)

# Step 4: Train the GNN

# Step 5: Evaluate the GNN
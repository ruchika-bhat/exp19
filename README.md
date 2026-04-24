AIM: REAL WORLD AND INTERACTIVE VISUALIZATIONS


THEORY:
In this experiment, we implemented different types of data visualizations using Python, where each graph was created using specific libraries and commands.
The goal was to understand not just the graphs, but also how the code works behind them.

First, we imported important libraries like:

Pandas (pd) → used to create and manage datasets in table form (DataFrame).
Plotly (px / go) → used for interactive graphs like treemap, Sankey, and 3D plots.
Matplotlib (plt) → used for basic plotting like radar charts.
SciPy (linkage, dendrogram) → used for hierarchical clustering.

# Treemap Code Explanation:
We created data using a dictionary and converted it into a DataFrame using pd.DataFrame().
Then:
px.treemap() → used to create the treemap
path → defines hierarchy (like Department → Subcategory)
values → decides size of each block
title → adds heading

This shows how hierarchical data is visually divided based on values.

# Dendrogram (Hierarchical Clustering):

np.random.rand() → generates random dataset
linkage(data, method='ward') → groups similar data points
dendrogram() → draws the tree-like structure

This helps understand how data points are clustered step-by-step.

# Venn Diagram Code:
venn2([set1, set2], set_labels=(...)) → creates diagram
Sets are used to represent groups
Overlapping area shows common elements

Useful for comparing similarities between two datasets.

# Sankey Diagram Code:
go.Sankey() → creates flow diagram
node → defines labels (like stages)
link → defines flow between nodes
source → starting point
target → ending point
value → quantity of flow

This clearly shows movement of data from one stage to another.

# 3D Scatter Plot Code:
px.scatter_3d() → creates 3D graph
x, y, z → represent three variables
color → differentiates data points

Helps analyze relationships between multiple variables at once.

# Radar Chart Code:
plt.subplots(polar=True) → creates circular plot
Angles are calculated using np.linspace()
Values are plotted and connected

Useful for comparing multiple attributes (like skills) in one view.


CONCLUSION:
This experiment not only demonstrated different types of data visualizations but also helped in understanding the logic
behind the code used to create them. It improved our ability to work with Python libraries and select appropriate graphs for different types of data.

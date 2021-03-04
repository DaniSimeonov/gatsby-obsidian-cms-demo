# Main Objective
The objective of this library is to create a tool that can visualise hierarchical data using an HTML5 canvas. Data should be serialized to and from the canvas via JSON. 

There should be distinct objects for the following: 

- Graph Nodes - Items in the flow chart / tree diagram
- Graph Links - connections between items in the chart: These need to 
- Graph Groups - collections of graph nodes or links used for homogeneous styling

![[interactive-flowchart.mp4]]

There should be event handlers that allow for expanding and collapsing nodes as well as sections of the graph.
- click 
- hover

The graph will have origin nodes with fixed positioning, from which the graph grows in a relative manner, allowing for dynamic movement through animations.

 ## Graph Nodes
 A graph node will be an item in the graph, with styling properties as well as content. It will also have animation transformation methods attached to it, which will be complex in the sense that a node's transformation needs to translate to all other nodes and links that are relative to it. 
 
 - Node center
 - Node Connection points
 - Node Shape
 - Node States as well as animated transition
	 - Expanded/collapsed
	 - content of each
	 - Styles of each
	 - Respected by related nodes and links!
 
 ## Graph links
 - line properties
 - symbol at end or beginning
 - active state
 - mathematical mapping of pathing and curves to make smooth lines between nodes, probably bezier curves 

Main difficulty wiht links will be how to programatically path them aesthetically and consistently.

## Graph groups
Groups should be objects that nodes and links can inherit from, and should be used to group homogenously styled items.

- Shape
- Border
- Fill
- Animation effect from state 1 to state 2
 
 
 
 


# Graph-Neural-Networks

### Graph Learning

The versatility of Graphs makes them a popular choice in various domains, including the following:

- Computer Science -> graphs can be used to model the structure of a computer program, making it easier to understand how different components of a system interact with each other

- 

For Example, images can be represented as a graph. Each pixel is a node, and edges represent relationships between neighboring pixels.

![](/Graph%20Image%201.png)


This allows for the application of graph-based algorithms to image processing and computer vision tasks.

### Why **Graph Learning**?

Graph Learning is the application of machine learning techniques to graph data. This study area encompasses a range of tasks aimed at understanding and manipulating graph-structured data. There are many graph learning tasks like -

1. **Node Classification** is a task that involves

---

## Why Graph Neural Networks?

Graph Neural Networks are the deep learning family of Graph Learning Techniques.

GNNs are a new category of deep learning architecture and are specifically designed for graph-structured data.

Unlike traditional deep learning algorithms, which have been 
primarily developed for text and images, GNNs are explicitly made to process and analyze graph datasets.

#### How do GNNs work?

Let's consider Node Classification Task in a social network. In a node classification task, GNNs take advantage of information from different sources to create a vector representation of each node in the graph.

This representation encompasses not only the original node features (such as name, age and gender) but also information from edge features (such as the strength of relationship between nodes) and global features (such as network-wide statistics)

This is why GNNs are more efficient than traditional ML Techniques on Graphs.

Instead of being limited to the original attributes, GNNs enrich the original node features with attributes from neighboring nodes, edges and global features, making the representation much more comprehensive and meaningful. The new node representations are then used to perform a specific task, such as node classification, regression, or link prediction.

Specifically, GNNs define a graph convolution operation that aggregates information from the 
neighboring nodes and edges to update the node representation. This operation is performed iteratively, 
allowing the model to learn more complex relationships between nodes as the number of iterations 
increases.

Example

---

# Graph Theory

Graph theory is a fundamental branch of mathematics that deals with the study of graphs and networks. 
A graph is a visual representation of complex data structures that helps us understand the relationships 
between different entities. Graph theory provides us with tools to model and analyze a vast array 
of real-world problems, such as transportation systems, social networks, and internet connectivity.

# Graph-Neural-Networks

### Graphs

A graph is a visual representation of a collection of **nodes** (**vertices**) and **edges** that connect these nodes, providing a structure to represent entities and their relationships.

Diag

### Graph Learning

The versatility of Graphs makes them a popular choice in various domains, including the following:

- **Computer Science** -> graphs can be used to model the structure of a computer program, making it easier to understand how different components of a system interact with each other

- **Physics**

- **Biology**

- ***Finance***

- **Engineering** -> Where graphs can be used to model and analyze complex systems, such as transportation networks and electical power grids.



Graphs are a natural representation of relational structures like those in social networks where the nodes are users and edges represent friendships.

But since, graphs are so versatile they can also be applied to domains where the underlying relational structure is less natural thus unlocking new insights, understanding and ways of learning about data.



For Example, images can be represented as a graph. Each pixel is a node, and edges represent relationships between neighboring pixels.

![](/Graph%20Image%201.png)


This allows for the application of graph-based algorithms to image processing and computer vision tasks.



Similarly, a sentence can be transformed into a graph, where nodes are words and edges represent relationships between adjacent workds. This appraoch is useful in natural language processing and information retrieval tasks, where the context and meaning of words are critical factors.



**Graphs** (unlike Texts and Images) do not have a fixed structure.

This flexibility also makes graphs more challenging to handle. The absence of a fixed structure means they can have an arbitrary  number of **nodes** and **edges**, with no **specific ordering**. 

In addition, graphs can represent dynamic data, where the connections between entities can change over time. 

For example, the relationships between users and products can change as they interact with each other. In this scenario, nodes and edges are updated to reflect changes in the real world, such as new users, new products, and new relationships.

### Why **Graph Learning**?

Graph Learning is the application of **machine learning techniques** to **graph data**. This study area encompasses a range of tasks aimed at understanding and manipulating graph-structured data. There are many graph learning tasks like -

1. **Node Classification** is a task that involves
2. **Link Prediction**
3. **Graph Classifications**
4. **Graph Generation**



#### Familites of Graph Learning Techniques

- Graph Signal Processing: which applies traditional signal processing methods to graphs, such as the Graph Fourier Transform and Spectral Analaysis. These techniques reveal the intrinsic properties of the graph, such as its connectivity and structure.

- Matrix Factorization, which seeks to find low-dimensional representations of large matrices. The goal of matrix factorization is to identify latent factors or patterns that explain the observed relationship in the original matrix. This approach can provide a compact and interpretable representation of the data.

- Random Walk, which refers to a mathematical concept used to model the movement of entities 
  in a graph. By simulating random walks over a graph, information about the relationships 
  between nodes can be gathered. This is why they are often used to generate training data for
  machine learning models.

- Deep Learning, which is a subfield of machine learning that focuses on neural networks with 
  multiple layers. Deep learning methods can effectively encode and represent graph data as 
  vectors. These vectors can then be used in various tasks with remarkable performance.

It is important to note that these techniques are not mutually exclusive and often overlap in their 
applications. In practice, they are often combined to form hybrid models that leverage the strengths of 
each. For example, matrix factorization and deep learning techniques might be used in combination 
to learn low-dimensional representations of graph-structured data.



### Representation: The Dataset

Traditional Tabular Datasets, such as spreadsheet, represent data as rows and columns with each row representing a single data point. However, in many real-world scenarios, the relationship between data points are just as meaningful as the data points themselves <Topology>

This is where graph datasets come in. Graph Datasets represent data points as nodes in a graph and the relationships between those data points as edges.



Diag Table



---

## Why Graph Neural Networks?

Graph Neural Networks are the deep learning family of Graph Learning Techniques.

GNNs are a new category of deep learning architecture and are specifically designed for graph-structured data.

Unlike traditional deep learning algorithms, which have been primarily developed for text and images, GNNs are explicitly made to process and analyze graph datasets.

diag

#### How do GNNs work?

Let's consider Node Classification Task in a social network. In a node classification task, GNNs take advantage of information from different sources to create a vector representation <embeddings> of each node in the graph.

This representation encompasses not only the original node features (such as name, age and gender) but also information from edge features (such as the strength of relationship between nodes) and global features (such as network-wide statistics).



This is why GNNs are more efficient than traditional ML Techniques on Graphs.

Instead of being limited to the original attributes, GNNs enrich the original node features with attributes from **neighboring nodes, edges and global features**, making the representation much more comprehensive and meaningful. The new node representations are then used to perform a specific task, such as node classification, regression, or link prediction.



Specifically, GNNs define a **graph convolution operation** that aggregates information from the neighboring nodes and edges to update the node representation. 

This operation is performed iteratively, allowing the model to learn more complex relationships between nodes as the number of iterations increases.

Example





##### Importance of Learning

More generally, GNNs, like other deep learning techniques, are most effective when applied to 
specific problems. These problems are characterized by high complexity, meaning that learning good 
representations is critical to solving the task at hand. For example, a highly complex task could be 
recommending the right products among billions of options to millions of customers. On the other 
hand, some problems, such as finding the youngest member of our family tree, can be solved without 
any machine learning technique.



Furthermore, GNNs require a substantial amount of data to perform effectively. Traditional machine 
learning techniques might be a better fit in cases where the dataset is small, as they are less reliant on 
large amounts of data. However, these techniques do not scale as well as GNNs. GNNs can process 
bigger datasets thanks to parallel and distributed training. They can also exploit the additional 
information more efficiently, which produces better results.

---

# Graph Theory

Graph theory is a fundamental branch of mathematics that deals with the study of graphs and networks. 
<<<<<<< HEAD
A graph is a visual representation of complex data structures that helps us understand the relationships between different entities. Graph theory provides us with tools to model and analyze a vast array of real-world problems, such as transportation systems, social networks, and internet connectivity.



```python
print("Hello World")
```
=======
A graph is a visual representation of complex data structures that helps us understand the relationships 
between different entities. Graph theory provides us with tools to model and analyze a vast array 
of real-world problems, such as transportation systems, social networks, and internet connectivity.
>>>>>>> 25c5c4f231d4de9c0db199d3794296973bac90e5

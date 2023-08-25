# Node Representations with DeepWalk

**Deep Walk** introduces important concepts such as **embeddings** that are at the core of GNNs. Unlike traditional neural networks, the goal of this **architecture** is to produce **representations** that are then fed to other models, which perfrom downstream tasks (for example, node classification). DownStream tasks are tasks that depend on output of pre - calculated value of a function / task. So, for node classification we already need neighbour nodes to be classified / calculated.



| 1. Introducing Word2Vec          |
| -------------------------------- |
| **2. DeepWalk and Random Walks** |
| **3. Implementing Deep Walk**    |

## Word2Vec

**Word2Vec** is a major component of DeepWalk Algorithm.

It proposes a new technique to translate words into vectors (also known as **embeddings**) using large datasets of text. These representations can then be used in downstream tasks, such as sentiment classification. It is also one of the rare examples of patented and popular ML architecture.



Here are a few examples of how Word2Vec can transfrom words into vectors:  

vec(king) = [-2.1, 4.1, 0.6]

vec(queen) = [-1.9, 2.6, 1.5]

vec(man) = [3.0, -1.1, -2]

vec(woman) = [2.8, -2.6, -1.1]



We notice that in terms of Euclidean Distance, the word vectors for king and queen are closer than the ones for king and woman. In general, other metrics, such as the popular **cosine similarity**, are used to measure the likeness of these words. Cosine Similarity focuses on the angle between the vectors and does not consider their magniture (length), which is more helpful in comparing them. It is defined as the follows :

$$
cosine similarity(A, B) = cos(theta) = A.B/normA. norm B
$$





One of the most surprising results of Word2Vec is ability to solve analogies. A popular example is how it can answer the question "man is to woman, what king is to ____?" It can be calculated as follows :

$$
vec(king) - vec(man) + vec(woman) ~nearly= vec(queen)
$$



This is not true with any analogy, but this property can bring interesting applications to perform arithmetic operations with embeddings.



## CBOW versus Skip-gram

A model must be trained on a pretext task to produce these vectors. The task itself does not need to be meaningful: its only goal is to produce high-quality embeddings. In practice, this task is always related to predicting words given a certain context.



Two architectures with similar tasks:

##### The contiguous bag-of-words (CBOW) model

    This is trained to predict a word using its surrounding context(words coming before and after the target word). The order of context words does not matter since their embeddings are summed in the model. The authors claim to obtain better results using four words before and after the one that is predicted.



##### The Continuous skip-gram model

    Here, we feed a single word to the model and try to predict the words around it. Increasing the range of context words leads to better embeddings but also increases the training time.

---Diag---

In general, the CBOW model is considered faster to train, but the skip-gram model is more accurate 
thanks to its ability to learn infrequent words. This topic is still debated in the NLP community: a 
different implementation could fix issues related to CBOW in some contexts.



### The skip-gram model

The goal of Word2Vec is to produce high-quality word embeddings. To learn these embeddings, the training task of the skip-gram model consists of predicting the correct context words given a target word.



--Maths--

$$
\sum 

$$

















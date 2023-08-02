# Facebook-Friend-Recommendation

In the context of social linkage or social network analysis, various similarity measures are used to quantify relationships between individuals or entities within a network. These measures help identify connections, assess similarity, and infer potential links in social networks. Some common similarity measures used for social linkage problem statements include:

- **1. Jaccard Similarity**: Measures the proportion of shared neighbors between two individuals relative to the total number of neighbors they have. It's particularly useful for binary relationships, like shared interests or connections.

- **2. Cosine Similarity:** Quantifies the cosine of the angle between two vectors representing individuals' attributes or behaviors. It's often applied to feature-based representations, such as user profiles or document vectors.

- **3. Pearson Correlation Coefficient:** Assesses the linear correlation between two individuals' attributes. It's useful for measuring similarity when the data is continuous and has a linear relationship.

- **4. Euclidean Distance:** Calculates the straight-line distance between two individuals' attribute values. It's commonly used when comparing numeric attributes.

- **5. Hamming Distance:** Measures the proportion of attributes that differ between two binary vectors. It's useful for comparing categorical attributes.

- **6. Graph-based Measures:** Commonly used in social network analysis, these measures consider the structure of the network itself. Examples include the Adamic/Adar index and the Katz similarity.

- **7. Overlap Coefficient:** Focuses on the intersection of attributes between two individuals, relative to the smaller set. It's effective for binary or categorical attributes.

- **8. Sørensen-Dice Coefficient:** Similar to the Jaccard index, it measures the overlap between two sets, but with a different weighting scheme.

- **9. Levenshtein Distance:** Often used for textual data, it calculates the minimum number of single-character edits (insertions, deletions, substitutions) required to transform one string into another.

- **10. Embedding-based Similarity:** With advancements in deep learning, embedding-based approaches like Word2Vec or node embeddings in graph networks can be used to quantify similarity.

## Diving deep into Graph Based measures

Graph-based similarity measures focus on leveraging the structure and connectivity of a social network to assess similarity or relatedness between individuals or entities. These measures consider how nodes (individuals) are connected and use properties of the network to quantify relationships. Here are some common graph-based similarity measures used in social network analysis:

- **1. Common Neighbors:** This measure counts the number of neighbors two nodes share in common. Nodes with more common neighbors are considered more similar.

- **2. Jaccard Coefficient:** Similar to the Jaccard similarity used for sets, this measure calculates the ratio of common neighbors to the total number of unique neighbors of two nodes.

- **3. Adamic/Adar Index:** It assigns higher similarity scores to nodes that share uncommon neighbors. It discounts the contribution of highly connected nodes, emphasizing the importance of nodes with fewer connections.

- **4. Preferential Attachment:** This measure is based on the assumption that nodes with higher degrees (more connections) are more likely to be similar or related.

- **5. Katz Similarity:** Katz similarity considers both the number of common neighbors and the paths connecting them. Longer paths receive less weight, promoting the importance of shorter paths.

- **6. Hitting Time:** This measure quantifies the expected time it takes for a random walk to reach one node starting from another. Nodes with shorter hitting times are considered more similar.

- **7. Personalized PageRank:** Similar to regular PageRank, personalized PageRank computes a node's importance based on random walks, but it biases the random walk towards a specific target node. Nodes with higher personalized PageRank scores are more similar.

- **8. Rooted PageRank:** Rooted PageRank computes the probability that a random walk starting at one node will visit another node. It can be used to measure the influence or similarity between nodes.

- **9. SimRank:** SimRank assesses similarity based on a recursive approach: nodes are similar if their neighbors are also similar. It captures structural similarity patterns in the network.

- **10. Community-based Measures:** Measures such as the Modularity score or the Cosine Similarity of nodes' membership vectors in communities can quantify the similarity of nodes based on their community memberships.
    
Graph-based similarity measures offer insights into the local and global connectivity patterns within a social network, helping to identify relationships that might not be apparent from node attributes alone. These measures play a crucial role in understanding social structures, link prediction, and recommendation systems within social network analysis.

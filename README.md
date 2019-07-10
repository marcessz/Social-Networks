# Social-Networks
Supplementary data for the paper *On the structural properties of social networks and their measurement-calibrated synthetic counterparts* - M. Nagy, R. Molontay (2019)


## Source
The graphs are collected from the following sources: 
* [Network Repository](http://networkrepository.com), 
* [The Colorado Index of Complex Networks (ICON)](http://networkrepository.com),  
* [KONECT - The Koblenz Network Collection](http://konect.uni-koblenz.de/)

## Summary of Networks


| Domain | Description | Range of network size | Number of networks |
|-----------------|--------------------------------------------------------------|:---------------------------------------:|:--------------:|
| Friendship | Online social networks of <br> friendships (mostly Facebook) | 324-23,613 <br> (median: 4,065) | 58 |
| Communication | Retweet, email and <br> reply networks | 96-33,696 <br> (avg: 4,687 | 43 |
| Collaboration | Co-authorship and collaboration <br> networks (mostly scientific) | 86-21,363 <br> (median: 553) | 19 |



## Graph Measurements
The [data folder](./data) contains the spreadsheets which contain the calculated metrics of the 120 real networks. 

The calculated metrics are the following:
- **Assortativity** (the *Pearson correlation coefficient* of degree between pairs of linked nodes) <br> 
The assortativity coefficient is given by  $$r=\frac{\sum_{j,k}{j\cdot k (e_{j,k}-q_{j}q_{k})}}{\sigma_ q^2},$$ where the term $q_{k}$ is the mass function of the distribution of the remaining degrees (degree of the nodes minus one) and $j$ and $k$ indicates the remaining degrees. Furthermore, $e_{j,k}$ refers to the mass function of the joint probability distribution of the remaining degrees of the two vertices. 
Finally, $\sigma_q^2$ denotes the variance of the remaining degree distribution with mass function $q_k$  i.e. <a href="https://www.codecogs.com/eqnedit.php?latex=$\sigma_q^2&space;=&space;\sum_k&space;k^2q_k&space;-&space;\left(\sum_k&space;k&space;q_k&space;\right)^2$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$\sigma_q^2&space;=&space;\sum_k&space;k^2q_k&space;-&space;\left(\sum_k&space;k&space;q_k&space;\right)^2$" title="$\sigma_q^2 = \sum_k k^2q_k - \left(\sum_k k q_k \right)^2$" /></a>
- **Average clustering coefficient** (the average local clustering coefficient. The local clustering coefficient of a node  quantifies how close its neighbours are to being a clique), 
- **Average degree** (the mean of the degrees), 
- **Average path length** (average number of steps along the shortest paths for all possible pairs of nodes), 
- **Density** (measures how dense the graph is, i.e. it is the number of edges divided by the maximum possible number of edges), 
- **Global clustering coefficient** (the number of closed triplets over the total number of triplets (both open and closed)), 
- **Four interval degree probabilities** introduced in [this paper](https://ieeexplore.ieee.org/abstract/document/7000748) (quantifies the degree distribtuion of the graph),
- **Largest eigenvector centrality** (eigenvector centrality is a measure of the influence of a node in a network), 
- **Maximum degree** (the maximum of the degrees), 
- **Maximum edge betweenness centrality** (betweenness centrality is a measure of centrality in a graph based on shortest paths),
- **Maximum vertex betweenness centrality** (betweenness centrality is a measure of centrality in a graph based on shortest paths),
- **Number of edges**,
- **Number of nodes**, 
- **Pseudo diameter** (diameter is the greatest distance between any pair of vertices. Pseudo diameter is an approximation of the diameter)

The **correlation heatmaps** of the metrics together with some analysis can be found [here](./correlations.md).

A detailed description of the dataset and the metrics can be found in [*Data-driven Analysis of Complex Networks and their Model-generated Counterparts*](https://arxiv.org/abs/1810.08498)

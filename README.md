# Social-Networks
Supplementary data for the paper *On the Structural Properties of Social Networks and their Measurement-calibrated Synthetic Counterparts* - M. Nagy, R. Molontay (2019)

## How to Cite
```
@inproceedings{nagy2019structural,
  title={On the Structural Properties of Social Networks and their Measurement-calibrated Synthetic Counterparts},
  author={Nagy, Marcell and Molontay, Roland},
  booktitle={2019 IEEE/ACM International Conference on Advances in Social Networks Analysis and Mining (ASONAM)},
  year={2019},
  organization={IEEE}
  }
```

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
The assortativity coefficient is given by  <a href="https://www.codecogs.com/eqnedit.php?latex=$$r=\frac{\sum_{j,k}{j\cdot&space;k&space;(e_{j,k}-q_{j}q_{k})}}{\sigma_&space;q^2},$$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$$r=\frac{\sum_{j,k}{j\cdot&space;k&space;(e_{j,k}-q_{j}q_{k})}}{\sigma_&space;q^2},$$" title="$$r=\frac{\sum_{j,k}{j\cdot k (e_{j,k}-q_{j}q_{k})}}{\sigma_ q^2},$$" /></a> where the term <a href="https://www.codecogs.com/eqnedit.php?latex=$q_k$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$q_k$" title="$q_k$" /></a> is the mass function of the distribution of the remaining degrees (degree of the nodes minus one) and *j* and *k* indicate the remaining degrees. Furthermore, <a href="https://www.codecogs.com/eqnedit.php?latex=e_{j,k}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?e_{j,k}" title="e_{j,k}" /></a> refers to the mass function of the joint probability distribution of the remaining degrees of the two vertices. 
Finally, <a href="https://www.codecogs.com/eqnedit.php?latex=$\sigma_q^2$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$\sigma_q^2$" title="$\sigma_q^2$" /></a> denotes the variance of the remaining degree distribution with mass function <a href="https://www.codecogs.com/eqnedit.php?latex=$q_k$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$q_k$" title="$q_k$" /></a>   i.e. <a href="https://www.codecogs.com/eqnedit.php?latex=$\sigma_q^2&space;=&space;\sum_k&space;k^2q_k&space;-&space;\left(\sum_k&space;k&space;q_k&space;\right)^2$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$\sigma_q^2&space;=&space;\sum_k&space;k^2q_k&space;-&space;\left(\sum_k&space;k&space;q_k&space;\right)^2$" title="$\sigma_q^2 = \sum_k k^2q_k - \left(\sum_k k q_k \right)^2$" /></a> 
- **Average clustering coefficient** (the average local clustering coefficient. The local clustering coefficient of a node  quantifies how close its neighbours are to being a clique) <br>
The local clustering coefficient of vertex *v* is the fraction of pairs of neighbors of *v* that are connected over all pairs of neighbors of *v*. Formally:
<a href="https://www.codecogs.com/eqnedit.php?latex=C_{\text{loc}}(v)&space;=&space;\frac{|&space;\{(s,t)&space;\text{&space;edges}:&space;s,t&space;\in&space;N_v&space;\text{&space;and&space;}&space;(s,t)&space;\in&space;E|\}}{\deg(v)&space;(\deg(v)-1)}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?C_{\text{loc}}(v)&space;=&space;\frac{|&space;\{(s,t)&space;\text{&space;edges}:&space;s,t&space;\in&space;N_v&space;\text{&space;and&space;}&space;(s,t)&space;\in&space;E|\}}{\deg(v)&space;(\deg(v)-1)}" title="C_{\text{loc}}(v) = \frac{| \{(s,t) \text{ edges}: s,t \in N_v \text{ and } (s,t) \in E|\}}{\deg(v) (\deg(v)-1)}" /></a>
where <a href="https://www.codecogs.com/eqnedit.php?latex=N_v" target="_blank"><img src="https://latex.codecogs.com/gif.latex?N_v" title="N_v" /></a> is the neighbourhood  of the node *v* i.e. the vertices adjacent to *v*.

The average (local) clustering coefficient of a *G* graph is defined as:
<a href="https://www.codecogs.com/eqnedit.php?latex=\Bar{C}(G)&space;=&space;\frac{1}{n}\sum_{v\in&space;V(G)}&space;C_{\text{loc}}(v)," target="_blank"><img src="https://latex.codecogs.com/gif.latex?\Bar{C}(G)&space;=&space;\frac{1}{n}\sum_{v\in&space;V(G)}&space;C_{\text{loc}}(v)," title="\Bar{C}(G) = \frac{1}{n}\sum_{v\in V(G)} C_{\text{loc}}(v)," /></a> where *n* is the size of the graph.
- **Average degree** (the mean of the degrees) 
- **Average path length** (average number of steps along the shortest paths for all possible pairs of nodes) <br>
A path is a sequence of edges which connect a sequence of vertices. The distance <a href="https://www.codecogs.com/eqnedit.php?latex=d(u,v)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?d(u,v)" title="d(u,v)" /></a> between the vertices *u* and *v* is the length (number of edges) of the shortest path connecting them. The <a href="https://www.codecogs.com/eqnedit.php?latex=l_G" target="_blank"><img src="https://latex.codecogs.com/gif.latex?l_G" title="l_G" /></a> average path length of a graph *G* of size *n* is defined as:
<a href="https://www.codecogs.com/eqnedit.php?latex=l_G&space;=&space;\frac{1}{n(n-1)}\sum_{i\neq&space;j}&space;d(v_i,v_j)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?l_G&space;=&space;\frac{1}{n(n-1)}\sum_{i\neq&space;j}&space;d(v_i,v_j)" title="l_G = \frac{1}{n(n-1)}\sum_{i\neq j} d(v_i,v_j)" /></a>
- **Density** (measures how dense the graph is) <br>
Graph density *D* is the ratio of the number of edges of the graph divided by the number of edges of a complete graph with the same number of vertices, i.e: <a href="https://www.codecogs.com/eqnedit.php?latex=D&space;=&space;\frac{|E|}{\frac{1}{2}|V|(|V|-1)}." target="_blank"><img src="https://latex.codecogs.com/gif.latex?D&space;=&space;\frac{|E|}{\frac{1}{2}|V|(|V|-1)}." title="D = \frac{|E|}{\frac{1}{2}|V|(|V|-1)}." /></a>
- **Global clustering coefficient** (the number of closed triplets over the total number of triplets (both open and closed)), 
- **Four interval degree probabilities** introduced in [this paper](https://ieeexplore.ieee.org/abstract/document/7000748) (quantifies the degree distribtuion of the graph)
- **Largest eigenvector centrality** (eigenvector centrality is a measure of the influence of a node in a network), 
- **Maximum degree** (the maximum of the degrees) <br>
For a graph, the vector of eigenvector centralities <a href="https://www.codecogs.com/eqnedit.php?latex=\mathbf{c}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\mathbf{c}" title="\mathbf{c}" /></a> satisfies the eigenvector equation <a href="https://www.codecogs.com/eqnedit.php?latex=\mathbf{A}&space;\cdot&space;\mathbf{c}&space;=&space;\lambda_1&space;\mathbf{c}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\mathbf{A}&space;\cdot&space;\mathbf{c}&space;=&space;\lambda_1&space;\mathbf{c}" title="\mathbf{A} \cdot \mathbf{c} = \lambda_1 \mathbf{c}" /></a>, where <a href="https://www.codecogs.com/eqnedit.php?latex=\lambda_1" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\lambda_1" title="\lambda_1" /></a> is the largest eigenvalue of the graph's adjacency matrix  <a href="https://www.codecogs.com/eqnedit.php?latex=\mathbf{A}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\mathbf{A}" title="\mathbf{A}" /></a>. In other words, for a connected undirected graph, the vector of eigenvector centralities is given by the (suitably normalized) eigenvector of corresponding to the largest eigenvalue of the adjacency matrix. 
- **Maximum vertex betweenness centrality** (betweenness centrality is a measure of centrality in a graph based on shortest paths) <br>
The betweenness centrality of a node *v* is given by the expression:
<a href="https://www.codecogs.com/eqnedit.php?latex=g(v)&space;=&space;\sum_{s&space;\neq&space;v&space;\neq&space;t}&space;\frac{\sigma_{st}(v)}{\sigma_{st}}," target="_blank"><img src="https://latex.codecogs.com/gif.latex?g(v)&space;=&space;\sum_{s&space;\neq&space;v&space;\neq&space;t}&space;\frac{\sigma_{st}(v)}{\sigma_{st}}," title="g(v) = \sum_{s \neq v \neq t} \frac{\sigma_{st}(v)}{\sigma_{st}}," /></a> where <a href="https://www.codecogs.com/eqnedit.php?latex=\sigma_{st}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\sigma_{st}" title="\sigma_{st}" /></a> is the total number of shortest paths from node *s* to node *t* and <a href="https://www.codecogs.com/eqnedit.php?latex=\sigma_{st}(v)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\sigma_{st}(v)" title="\sigma_{st}(v)" /></a> is the number of those paths that pass through *v*.
- **Maximum edge betweenness centrality** (betweenness centrality is a measure of centrality in a graph based on shortest paths) <br>
The edge betweenness centrality of an edge is the number of shortest paths between pairs of vertices that run along it. In other words this is analogous to the previously defined <a href="https://www.codecogs.com/eqnedit.php?latex=\sigma_{st}(v)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\sigma_{st}(v)" title="\sigma_{st}(v)" /></a>, but here we consider an edge instead of a node.
- **Number of edges**
- **Number of nodes** (size of the network) 
- **Pseudo diameter** (diameter is the greatest distance between any pair of vertices. Pseudo diameter is an approximation of the diameter)

The **correlation heatmaps** of the metrics together with some analysis can be found [here](./correlations.md).

A detailed description of the dataset and the metrics can be found in [*Data-driven Analysis of Complex Networks and their Model-generated Counterparts*](https://arxiv.org/abs/1810.08498)

# Social-Networks
Supplementary data for the paper *On the structural properties of social networks and their measurement-calibrated synthetic counterparts* - M. Nagy, R. Molontay (2019)
## How to Cite
```
@article{nagy2019social,
  title={On the structural properties of social networks and their measurement-calibrated synthetic counterparts},
  author={Nagy, Marcell and Molontay, Roland},
  journal={arXiv preprint arXiv:1810.08498},
  url={https://arxiv.org/abs/1810.08498},
  year={2019}
}
```


## Source
The graphs are collected from the following sources: 
* [Network Repository](http://networkrepository.com), 
* [The Colorado Index of Complex Networks (ICON)](http://networkrepository.com),  
* [KONECT - The Koblenz Network Collection](http://konect.uni-koblenz.de/)

## Summary of Networks


The edgelists of the graphs can be found in the [graphs folder](./graphs).

| Domain | Description | Range of network size | Number of networks |
|-----------------|--------------------------------------------------------------|:---------------------------------------:|:--------------:|
| Friendship | Online social networks of <br> friendships (mostly Facebook) | 50-2,995 <br> (avg: 946) | 100 |
| Communication | Retweet, email and <br> reply networks | 44-125 <br> (avg: 55) | 100 |
| Collaboration | Co-authorship and collaboration <br> networks (mostly scientific) | 19-1,500 <br> (avg: 118) | 18 |



## Graph Measurements
The [data folder](./data) contains a spreadsheet that contains the calculated metrics of the 120 real networks. 

The calculated metrics are the following:
- assortativity, 
- average clustering coefficient, 
- average degree, 
- average path length, 
- density, 
- global clustering coefficient, 
- four interval degree probabilities introduced in [this paper](https://ieeexplore.ieee.org/abstract/document/7000748),
- largest eigenvector centrality, 
- maximum degree, 
- maximum edge betweenness centrality,
- maximum vertex betweenness centrality,
- number of edges,
- number of nodes, 
- pseudo diameter

A detailed description of the dataset and the metrics can be found in [*On the structural properties of social networks and their measurement-calibrated synthetic counterparts*](https://arxiv.org/abs/1810.08498)

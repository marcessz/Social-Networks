# Spearman's rank correlations of the metrics

We have normalized the average path length, maximum degree and pseudo diameter metrics before calculating the correlations as follows: 
* ```avg_path_log = avg_path_length / log(size)```
* ```max_deg_n = max_deg / (size - 1)```
* ```p_diam_log = pseudo_diam / log(size)```

Corrleation heatmap of the friendship networks:
![heatmap_friendship](./heatmap_friend.png "Correlation heatmap of metrics on friendship networks")

Correration heatmap of the communication networks:
![heatmap_comm](./heatmap_comm.png "Correlation heatmap of metrics on communication networks")

Correlation heatmap of the collaboration networks:
![heatmap_collab](./heatmap_collab.png "Correlation heatmap of metrics on collaboration networks")

The metris are hierarchically-clustered using the following distance metric: <br>
<a href="https://www.codecogs.com/eqnedit.php?latex=d(p,q)&space;=&space;\sum_{i=1}^{k}&space;\left&space;|&space;\left&space;|&space;p_i&space;\right&space;|&space;-&space;\left&space;|&space;q_i&space;\right&space;|&space;\right&space;|" target="_blank"><img src="https://latex.codecogs.com/gif.latex?d(p,q)&space;=&space;\sum_{i=1}^{k}&space;\left&space;|&space;\left&space;|&space;p_i&space;\right&space;|&space;-&space;\left&space;|&space;q_i&space;\right&space;|&space;\right&space;|" title="d(p,q) = \sum_{i=1}^{k} \left | \left | p_i \right | - \left | q_i \right | \right |" /></a>

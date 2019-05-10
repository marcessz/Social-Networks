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
![heatmap_collab](./heatmap_friend.png "Correlation heatmap of metrics on collaboration networks")



# Page Rank, Random Walks and Embeddings

* 4.1 Page Rank: [video](https://www.youtube.com/watch?v=TU0ankRcHmo&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=10&ab_channel=StanfordOnline)
  - Stochastic adj. matrix $\mathbf{M}$: $M_{i,j}=1/d_j$:
    $$1\cdot \mathbf{r}=\mathbf{M}\mathbf{r}$$
  - $r$ is the principle eigenvector or $\mathbf{M}$, or the stationary distribution of a random walk
* 4.2 PageRank: How to Solve? [video](https://www.youtube.com/watch?v=rK2ZBmQHVVs&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=11&ab_channel=StanfordOnline)
  * Power iteration
  * Issues:
    * Spider trap
    * Dead end
  * Solutions:
    * spider trap: random teleport with probability $\beta$
    * dead end: teleport with probability $1$
  * Google solution:
    * teleport at each step with probability $\beta$, where $\beta$ ~ 0.8, 0.9
* 4.3 Random walk with Restarts [video](https://www.youtube.com/watch?v=HbzQzUaJ_9I&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=12&ab_channel=StanfordOnline)
  * PageRank: random teleport to any nodes
  * Personalized PageRank: teleport to subset nodes $S$
  * Random walks with Restarts: teleport to the starting nodes $S={Q}$
* 4.4 Matrix factorization and node embeddings
  * Node2vec can also be formulated as a metrics factorization!
  * Limitation of node embedding via matrix factorization and random walks
    * When new node joined, we need to recalculate the embeddings
    * Cannot capture structure similarity
    * Cannot unitize node, edge, and graph features
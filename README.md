## Hi 👋

[This](https://github.com/jianboli/CS224W-Fall-2021-Stanford) is a fork of MartinLwx's work on the Machine Learning with Graphs in Stanford.

The official site: <https://web.stanford.edu/class/cs224w/>

## Resources

🎥: https://www.youtube.com/playlist?list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn

🏷 && ⌨️: https://web.stanford.edu/class/cs224w/

## Progress track

- [X] 1. Introduction (https://web.stanford.edu/class/cs224w/slides/01-intro.pdf)
  - 1.1 Why Graphs: [video](https://www.youtube.com/watch?v=JAB_plj2rbA&ab_channel=StanfordOnline)
  - 1.2 Applications of Grapha ML: [video](https://www.youtube.com/watch?v=aBHC6xzx9YI&ab_channel=StanfordOnline)
  - 1.3 Choice of Graph Representations: [video](https://www.youtube.com/watch?v=P-m1Qv6-8cI&ab_channel=StanfordOnline)
- [ ] 2. Traditional Methods for Machine Learning in Graphs (In the 2023 class, this charpter has been deleted)
  - 2.1 Traditional Feature-based Methods: Node
    - Degree:
    - Centrality:
        - Eignvector centrality:
            - my centrality is a constant times the average centrality of my neighors
            - the centrality is then a eigen vector
        - Betweenness centrality:
            - how many shortest parths of any two pair of nodes goes through me
        - Closeness centrality:
            - 1/(sum of my shortest distance to all the other nodes)
            - Question: the farest nodes might dominants the sum, deminish the impact of local structure
    - Clustering coefficient:
        - density of edges among my neighor nodes (how my direct friends knows each other)
        - count of triangles - graphlets
    - Graphlets:
        - dispit the same pattern, my location could lead to different graphlets, e.g. in the graphlet, 1 <-> 2 <-> 3, if I am 1 is different from I am 2
        - Graphlet degree vector (GDV)
  - 2.2 Traditional Feature-based Methods: Link
    - CS224W: Machine Learning with Graphs | 2021 | Lecture 2.1 - Traditional Feature-based Methods: Node [video](https://www.youtube.com/watch?v=3IS7UhNMQ3U&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=4&t=1s&pp=iAQB)
    * Lecture 2.2 - Traditional Feature-based Methods: [video](https://www.youtube.com/watch?v=4dVwlE9jYxY&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=5)


## Colabs

- [ ] [Colab 0](./CS224W_Colab_0.ipynb)
- [ ] [Colab 1](./CS224W_Colab_1.ipynb)
- [ ] [Colab 2](./CS224W_Colab_2.ipynb)
- [ ] [Colab 3](./CS224W_Colab_3.ipynb)
- [ ] [Colab 4](./CS224W_Colab_4.ipynb)
- [ ] [Colab 5](./CS224W_Colab_5.ipynb)

## Highlights

- Message passing in GraphML. *I think it is the most important conception in GNN. The ppts are very intuitive and concise which are quite worth reading*
- PyG. *In the Colabs, we will use this package quite often, not only at high-level but also at low-level. To finish the Colabs, you usually need to check the docs, which make you familiar with PyG*
- GCN/GAT/GraphSAGE *We will implement these models in the Colabs*
- PageRank, Knowledge graph, etc. *This course covers many topics in GNN.*



## Looking for answers for other cs-courses ?

:hugs: Welcome to check my repo [cs-courses](https://github.com/MartinLwx/cs-courses).

Join me and enjoy the journey :rocket:

# Label Propagation for Node Classification

* 5.1 Message passing and Node Classification: [video](https://www.youtube.com/watch?v=6g9vtxUmfwM&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=14&ab_channel=StanfordOnline)
  * Message passing and Node Classification
    * Relational classification
    * Iterative classification
    * Belief propagation
  * Main types of dependencies that lead to correlation:
  * Homophily: the tendency of individuals to associate and bond with similar other
  * Influence: social connections can influence the individual characteristics of a person
  * Motivation: similar nodes are typically close together or directly connected
  * Collective Classification
    * Local Classifier
    * Relational Classifier
    * Collective Classifier
* 5.2 Relational and Iterative Classification: [video](https://www.youtube.com/watch?v=QUO-HQ44EDc&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=15)
  * Relational classification
    * Purely based on neighbor's probability of to be a label
  * Iterative classification (two classifiers)
    * Phase 1: classify based on node attributes alone
      * train classifier $\phi_1(f_v)$ to predict based on $f_v$:
        * own features -> predictive models -> own label -> neighbor summary factor $z_v$ (manually picked function based on the neighbor label)
      * train classifier $\phi_2(f_v, z_v)$ to predict $Y_v$:
        * neighbor feature summary $z_v$ & own features $f_v$ -> update own label
    * Phase 2: 
      * On test set, 
      * set label $Y_v$ using $\phi_1$
      * iterate the following two steps until converge or reaches maximum iteration
        * compute $z_v$ 
        * update $Y_v$ based on $\phi_2$
    * **Note**: convergence is not guaranteed!
* 5.3 Collective Classification: belief propagation [video](https://www.youtube.com/watch?v=kh3I_UTtUOo&list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn&index=16)
  * 
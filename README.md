# Wikipedias-PageRank
In this work, the objective was to program the Page Rank algorithm in a parallelized way (with PySpark).
Concretely I worked on the platform of DataBricks, which is very useful in order to work with Spark (https://community.cloud.databricks.com).

For attaining a parallelized structure, I used several PySpark Structures which perform the computations in a Parallelize way.
Since I did not have the resources to run the Page Rank algorithm on the entire WikiPedia, I only ran it on a fraction of it (0.001). 
Anyway, the code is structured in such a way that it could be executed by several devices at the same time. 
My advice for running the notebook, is to create an account on DataBricks, load the Notebook there and execute it (Maybe in other platforms such us Google Colab does work too).


## Page Rank Algorithm 

### Concept
The PageRank algorithm outputs a probability distribution used to represent the likelihood that a person randomly clicking on links will arrive at any particular page. PageRank can be calculated for collections of documents of any size. It is assumed in several research papers that the distribution is evenly divided among all documents in the collection at the beginning of the computational process. The PageRank computations require several passes, called “iterations”, through the collection to adjust approximate PageRank values to more closely reflect the theoretical true value.

<p align="center">
  <img src="https://imgr.search.brave.com/_WnLnLT7yMNqv0EQMJ7VbWrRI77-rWLtx2YhCDwdTlI/fit/500/403/ce/1/aHR0cDovL3d3dy5k/aWFsbWUuY29tL2Js/b2cvd3AtY29udGVu/dC91cGxvYWRzLzIw/MTEvMDYvcGFnZXJh/bmsyLmpwZw" alt="Sublime's custom image"/>
</p>


### Resources

(for getting the basic notions)
- https://www.geeksforgeeks.org/page-rank-algorithm-implementation/   
- https://www.youtube.com/watch?v=P8Kt6Abq_rM&t=243s   
- https://towardsdatascience.com/pagerank-algorithm-fully-explained-dc794184b4af

(deeper papers)
- https://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=B955F5D6E7EC957FC67CCF4F0B9F8183?doi=10.1.1.38.5427&rep=rep1&type=pdf
- https://web.stanford.edu/class/cs54n/handouts/24-GooglePageRankAlgorithm.pdf

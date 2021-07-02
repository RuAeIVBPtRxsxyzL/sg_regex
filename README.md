<meta name="robots" content="noindex">
# Subgraph Regex

We collect all code and data for the Node Embedding with Semantic Subgraphs project here. This work in created in association with our publication, <b>CompactWalks: Taming Knowledge-Graph Embeddings with Domain- and Task-Specific Pathways</b>. If you find this repository helpful towards the development of novel methods and systems, please cite our work. The layout of this repo is as follows:

In the directory <b>Code</b> we have the following:

<ul>
  <li><b>Subgraph_Regex.ipynb</b>: This is a Jupyter Notebook containing all of the Python code for the CompactWalk project. The Notebook is divided into multiple sections. The first section covers how we create and utilize regular expression grammar in our project. This section heavily utilizes the <a href="https://github.com/lark-parser/lark">lark</a> grammar parasing library. The following section focuses on leveraging the grammar and constructed queries to extract patterns from existing graph databases. This section focuses on CYPHER query generation and Neo4J database connections. The final section of the notebook contains code for performing machine learning tasks on semantic subgraph creation; performing semantic walks on these subgraphs, and calculation of embedding values for these graph.</li>
</ul>


In the directory <b>Data</b> we have the following:
<ul>
  <li><b>regex_build_times.csv</b>: A dataset of the times taken to build various subgraphs. In this dataset, the length of time to gather and build a subgraph with naive methods with one utilizing semantic filtering. Details of the methods are discussed more elaborately in our publication.</li> 
  <li><b>results.xlsx</b>: A collection of the MRR and Hits@k values. These values are calculated for three different embedding methodologies; deepwalk, node2vec, metapath2vec in three different settings: the whole graph, non-semantic graph (-NS), and semantic graph (-SS).</li>
  <li><b>robokop-2d.emb</b>: Two dimensional node2vec embeddings run on the ROBOKOP subgraph. These embeddings were generated using the 
    <a href="http://snap.stanford.edu/">SNAP: Stanford Network Analysis Project</a>. </li>
 
</ul>

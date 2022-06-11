# Network Embeddings

This is a school project realized for a Machine Learning Course at AGH University of Science and Technology. The main purpose of the project is to examine network data representation with the use of network embeddings.

### Project Authors
- Jan Ściga
- Michał Kurdziel
- Szymon Bobrowski

#### New contributions were added to the project in the following order:
1. Get acquainted with the subject of Network Embeddings
2. Configure appropriate cloud environment (Google Colab and Github)
3. Use Node2Vec algorithm to create network embeddings
4. Use t-SNE to reduce the number of dimensions in received embeddings
5. Visualize data using proper python libraries
6. Examine properties of other embedding algorithms (LINE, Deepwalk, SDNE, Struct2Vec)
7. Customize Node2Vec implementation to test various scenarios
8. Predict the link type based on embeddings
9. Combine link prediction with algorithm comparison
10. Examine how embedding vector size impacts link prediction


## File content

### node2vec_demo.ipynb
This file contains a demonstration of a simple network embeddings model. First, we create network embeddings using Node2Vec. Then we narrow down vector dimension to two with help of t-SNE, so that we can visualize the data on a graph.

### embedding_alg_evaluation.ipynb
In this notebook, we compare different network algorithms considering two factors; visual node representation (after size reduction) as well as execution time. The following algorithms are examined:
- DeepWalk
- LINE
- Node2Vec
- SDNE
- Struc2Vec

### collab_main.ipynb
This is a simple neural network model using network embeddings created with Node2Vec or DeepWalk (depending on file configuration) for link prediction. To use Node2Vec uncomment line _X_embed = node2vec_get_embeddings(X)_ and comment out _X_embed = deepwalk_get_embeddings(X)_. To use DeepWalk instead reverse the previous steps.

### embedding_length_vs_model_acc.ipynb
This file is _collab_main.ipynb_ execution in a loop with different embedding vector sizes for each loop. It is used to examine how embedding vector size impacts link prediction.


## How to run

### node2vec_demo.ipynb
1. Download ZIP with repo content
2. Open [Google Colab](https://colab.research.google.com)
3. Upload _node2vec_demo.ipynb_
4. Go to Table of contents -> Files and upload _as-rank.caida.peercones-with-IX-short.txt_
5. To run the code go to Runtime -> Run all

### embedding_alg_evaluation.ipynb
1. Download ZIP with repo content
2. Open [Google Colab](https://colab.research.google.com)
3. Upload _embedding_alg_evaluation.ipynb_
4. Go to Table of contents -> Files and upload _reference.rar_
5. To run the code go to Runtime -> Run all

### collab_main.ipynb
1. Download ZIP with repo content
2. Open [Google Colab](https://colab.research.google.com)
3. Upload _collab_main.ipynb_
4. Go to Table of contents -> Files and upload _copy.zip_ and _deepwalk_config.py_
5. To run the code go to Runtime -> Run all

### embedding_length_vs_model_acc.ipynb
1. Download ZIP with repo content
2. Open [Google Colab](https://colab.research.google.com)
3. Upload _embedding_length_vs_model_acc.ipynb_
4. Go to Table of contents -> Files and upload _copy.zip_ and _deepwalk_config.py_
5. To run the code go to Runtime -> Run all

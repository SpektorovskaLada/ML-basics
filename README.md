# Introduction to machine learning
Laboratory work on the discipline **"Introduction to ML"**
---
### Laboratory work #1
**Topic:** Basic skills in working in the Python environment
Task: Given an undirected graph G with V vertices, where the weights of the arcs dij are known for ∀i, j = 1, ..., V , i ̸= j. Construct a minimum spanning tree - a subgraph J of the graph G, using Prim's algorithm:
- Choose any vertex of the graph G and add it to J.
- Add to J the edge with the smallest weight that connects the vertex of the subgraph J with a vertex that does not belong to J.
- Perform step 2 until V − 1 edges are added to J.

### Laboratory work №2
**Topic:** Construction and assessment of the quality of a naive Bayesian model for classification using the Scikit-Learn Python library.
- Initial data:
- (a) sklearn.datasets.make_moons
- (b) sklearn.datasets.load_digits
- Data pre-adjusted to work with MultinomialNB (only positive values).
- Tasks:
- Construction of classification models (GaussianNB and MultinomialNB).
- Testing on training and validation sets.
- Assessment of overfitting.
- Calculation of posterior probabilities ('predict_proba').
- Conclusion:
- For 'make_moons', **GaussianNB** showed the best accuracy.
- For 'load_digits', the highest accuracy was demonstrated by **MultinomialNB**.
- In both cases, the accuracy on the test data was close to the training data → no overtraining is observed.
---

### Laboratory work #3
**Topic:** Data classification using neural networks
- Initial data:
- (a) sklearn.datasets.make_moons
- (b) sklearn.datasets.load_digits
- Task:
- Building classification models on training/validation sets.
- Experiments with the number of neurons in the hidden layer.
- Quality assessment: **confusion matrix**, precision, recall, F1-score.
- Building **PR-curves**, **ROC-curves**, calculating **AUC**.
- Conclusion: increasing the number of neurons affects the quality of the model; the optimal architecture allows achieving a stable data distribution without overtraining.

---

### Lab #4
**Topic:** Data Clustering
- Input data:
- make_blobs
- make_circles
- Tasks:
- Visualization of the original data.
- Building clustering models.
- Comparison of alternative models with changing parameters and distance metrics.
- Quality metrics (module 'sklearn.metrics'):
- Estimated Number of Clusters
- Adjusted Rand Index
- Silhouette Coefficient
- Davies–Bouldin Index
- Conclusion: the clusters are well separated; the indices confirm the correctness of the model even with different parameters.

---
### Lab #5
**Topic:** Building and evaluating ensembles of classification and regression models using the Scikit-Learn Python library
- Method: GradientBoostingRegressor
- Initial data: sklearn.datasets.load_diabetes
- Tasks:
- Build an ensemble of models using the given method.
- Compare the performance of the ensemble with individual models.
- Calculate the accuracy, bias, and variance.
- Conclusion: ensembles are more effective for tasks where high accuracy is required.

### Libraries used
- numpy
- pandas
- matplotlib
- scikit-learn
- seaborn

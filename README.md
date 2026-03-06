📌**Assignment Overview.**

The objective of this assignment is to explore different techniques used in large-scale similarity detection. The implementation covers:
- Construction of k-grams for document representation
- Computation of exact Jaccard similarity between documents
- Approximation of similarity using MinHash signatures
- Identification of candidate pairs using Locality Sensitive Hashing (LSH)
- Application of these methods to the MovieLens 100K dataset

All experiments are implemented in Python using Jupyter Notebook.

📌**Tasks Implemented**

1.**K-Gram Construction**

Different types of k-grams were generated for four documents:
- Character 2-grams
- Character 3-grams
- Word 2-grams

Using these representations, Jaccard similarity was computed between all document pairs to analyze how different representations affect similarity estimation.

2. **MinHashing**

MinHash signatures were generated for document pairs using different numbers of hash functions. Experiments were conducted using:
- 20 hash functions
- 60 hash functions
- 150 hash functions
- 300 hash functions
- 600 hash functions

The approximate Jaccard similarity obtained from MinHash signatures was compared with the exact Jaccard similarity.

3. **Locality Sensitive Hashing (LSH)**
   
Locality Sensitive Hashing was applied to efficiently detect document pairs with high similarity. The signature matrix was divided into bands and rows, and the probability of detecting candidate pairs was analyzed using the LSH S-curve model.

5. **MinHashing on MovieLens Dataset**

The MovieLens 100K dataset was used to compute similarity between users based on the set of movies they have rated.

📌**Steps performed:**

  1. Compute exact Jaccard similarity between users
  2. Generate MinHash signatures for users
  3. Estimate similarity using signatures
  4. Analyze false positives and false negatives
  5. Experiments were conducted using:
     50 hash functions
     100 hash functions
     200 hash functions

5. **LSH on MovieLens Dataset**

Locality Sensitive Hashing was implemented on user signatures to identify candidate pairs efficiently.
Experiments were performed using different band configurations:

  r = 5, b = 10
  r = 5, b = 20
  r = 5, b = 40
  r = 10, b = 20

The results were analyzed using false positive and false negative statistics.

📌**Graphs Generated**

The following graphs were generated to analyze the behavior of LSH:
1. False Positives vs Similarity Threshold
2. False Negatives vs Similarity Threshold
These graphs help illustrate the trade-off between detection accuracy and filtering efficiency when using LSH.

📌**Technologies Used**

The project uses the following tools and libraries:

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

📌**Results:**
![False Positives](false_positive.png)
![False Negatives](false_negative.png)


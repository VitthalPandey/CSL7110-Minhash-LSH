📌**Assignment**: 
**MinHash and LSH Implementation**

📖 **Overview**

This assignment focuses on understanding and implementing similarity detection techniques using:
  1. k-Grams
  2. Jaccard Similarity
  3. MinHash
  4. Locality Sensitive Hashing (LSH)

The project is divided into two main parts:
  1. Similarity analysis on small text documents (D1–D4)
  2. Similarity detection among users in the MovieLens dataset
The goal is to study how approximate similarity methods behave compared to exact similarity computation.

🧠 **Concepts Implemented**

1️⃣ **k-Gram Similarity**

  1. Character 2-grams
  2. Character 3-grams
  3. Word 2-grams
  4. Exact Jaccard similarity computation
This part shows how similarity changes when the gram size increases.

2️⃣ **MinHash**
  1. Implemented multiple hash functions
  2. Compared estimated similarity with exact Jaccard similarity
  3. Tested different signature sizes (t = 50, 100, 200, etc.)
This section demonstrates how increasing signature size improves approximation accuracy.

3️⃣ **Locality Sensitive Hashing (LSH)**
  1. Banding technique applied
  2. Different (b, r) configurations tested
  3. False Positives and False Negatives analyzed
  4. Threshold values (0.6 and 0.8) evaluated
This section highlights how LSH parameters affect accuracy and filtering performance.

📊 **Key Observations**
1. Smaller k-grams produce higher similarity values.
2. Larger k-grams are more restrictive and reduce similarity.
3. Increasing the number of hash functions reduces variance in MinHash.
4. LSH performance is highly sensitive to band size (r).
5. Proper parameter tuning significantly reduces false positives.
![False Positives](false positive.png)
![False Negatives](false negative.png)

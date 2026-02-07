**Cold-Start Handling**

The system uses a hybrid recommendation strategy:

- For movies present in the dataset, recommendations are generated using TF-IDF–based content similarity.

- For new or unseen movies, a genre-based fallback strategy is applied to ensure meaningful recommendations without requiring immediate retraining.

This design enables low-latency inference and stable recommendations in early production stages (V1).

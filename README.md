Core Functionality
The script is built around the following methods:

get_distinct_words(corpus): Identifies and returns all unique words present in the corpus after converting text to lowercase and removing punctuation.

construct_co_occurrence_matrix(corpus, window_size=4): Creates a matrix that records how often pairs of words appear together within a specified window. The default window_size is 4 words before and 4 words after the central word.

perform_dimensionality_reduction(matrix, k_dimensions=2): Applies Principal Component Analysis (PCA) to reduce the dimensionality of the co-occurrence matrix, yielding k-dimensional word embeddings. For visualization, k is set to 2.

plot_vectors_2d(vectors, word_labels, title="2D Word Embeddings"): Visualizes the 2D word embeddings using matplotlib, plotting each word as a point and labeling it for semantic interpretation.

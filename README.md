# Book Recommendation System (WIP)

This project implements a book recommendation system using a combination of clustering and nearest neighbor algorithms. It uses the Goodreads dataset to recommend books based on user queries or selected books. The system leverages the KMeans clustering algorithm for grouping books and the k-Nearest Neighbors (kNN) algorithm for personalized recommendations.

## Features

- **Data Preprocessing:**
  - Removes outliers from the dataset to improve clustering accuracy.
  - Normalizes numerical features such as `average_rating`, `ratings_count`, and `num_pages` using Min-Max scaling.
  - Creates textual features from book titles and authors using TF-IDF vectorization.

- **Clustering:**
  - Uses the Elbow Method to determine the optimal number of clusters.
  - Applies KMeans clustering to group similar books.

- **Recommendation System:**
  - Implements a k-Nearest Neighbors model to recommend similar books.
  - Allows querying by full or partial book titles.

- **Visualization:**
  - Visualizes clusters and centroids for better interpretability.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/book-recommendation-system.git
   cd book-recommendation-system

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt

3. The dataset is automatically downloaded using the Kaggle API. Ensure you have the API key configured.


## Usage

1. Run the main script:
   ```bash
   python book_recommendation_system.py

2. Query recommendations by providing a book title:
   ```bash
   display_recommendations(book_title="The Catcher in the Rye") 

3. Search for books by partial title matches:
   ```bash
   search_books_by_partial_title("Harry Potter")


## Known limitations

- The recommendations are not always highly relevant and need improvement.
- Adjusting the feature selection or clustering parameters may improve the results.
- The dataset may have missing or inconsistent data, which can affect performance.

## Note

This project is a work in progress and is not yet perfected. Contributions and suggestions are welcome to enhance its functionality and performance.

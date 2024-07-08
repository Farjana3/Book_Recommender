# Book_Recommender
This project implements two types of book recommender systems: a popularity-based recommender and a collaborative filtering-based recommender.

## Data
The project uses three datasets:

  books.csv: Contains information about books.
  users.csv: Contains information about users.
  ratings.csv: Contains book ratings provided by users.
## Popularity-Based Recommender
	Data Merging: Combines book ratings with book details.
	Calculations:
					Counts the number of ratings per book.
					Computes the average rating per book.
	Filtering and Sorting: Selects books with at least 200 ratings and sorts them by average rating in descending order.
## Collaborative Filtering-Based Recommender
	Expert Users: Selects users who have rated more than 200 books.
	Popular Books: Selects books that have received at least 50 ratings from these expert users.
	Pivot Table: Creates a user-item matrix for these popular books.
	Cosine Similarity: Computes similarity scores between books.
R	ecommendation Function: Recommends books based on similarity to a given book.
## How to Use
	Load Data: Ensure the datasets are placed in the correct directory.
	Run the Script: Execute the provided script to generate recommendations.
	Get Recommendations: Use the recommend function to get book recommendations based on a given book title.
## Dependencies
	pandas
	numpy
	scikit-learn

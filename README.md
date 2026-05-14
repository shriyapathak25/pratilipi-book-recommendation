# Pratilipi Book Recommendation System

About the Project

This project is a simple book recommendation system built using Python.

The main goal of this project is to recommend new books to users based on their previous reading interactions. The recommendation logic is built using a content-based filtering approach where user preferences are identified using book genres.

Before building the model, I first explored the dataset carefully to understand user reading behavior. One important observation was that most users were reading only one chapter from a book and exploring multiple books instead of completely finishing one book. Because of this, I focused on recommending new books instead of predicting the next chapter.



# Files in this Repository
1. recommendation.ipynb
Main notebook containing complete EDA, recommendation logic, evaluation, and explanations.
2. chapters.csv
Contains book and chapter related information like genres, chapter sequence, author id, etc.
3. interactions.csv
Contains user interaction history with chapters and books.
4. user_recommendations.csv
Final generated recommendations for users.
5. user_recommendations
final recommendations output   



# Libraries Used
# The following Python libraries were used in this project:

1. pandas
2. numpy
3. scikit-learn
4. matplotlib
5. seaborn



# Recommendation Approach

I used a content-based recommendation system for this project.

The model creates a genre preference profile for each user based on the books they interacted with. Similarly, each book also gets a genre profile using its tags.

Cosine similarity is then used to compare user preferences with book profiles and recommend similar books.

For new users with no interaction history, the system recommends popular books as a fallback solution.



# How to Run the Project

# Option 1 — Run in Google Colab
1.Open recommendation.ipynb in Google Colab.
2.Upload the following files into the Colab session:
3.chapters.csv
  interactions.csv
4.Run all notebook cells from top to bottom.
5.Final recommendations will be generated and saved as:
user_recommendations.csv


# Option 2 — Run in VS Code or Local System
Install Python on your system.
Install the required libraries using:
pip install pandas numpy scikit-learn matplotlib seaborn
Open the project folder in VS Code.
Make sure these files are present in the same folder:
recommendation.ipynb
chapters.csv
interactions.csv
Run the notebook cells one by one using Jupyter Notebook support in VS Code.
The final output file will be saved as:
user_recommendations.csv

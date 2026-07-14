# 🎬 Movie Recommendation System using Apriori Algorithm

A movie recommendation system built using the **Apriori algorithm** and **association rule mining** on the MovieLens dataset. Instead of using traditional collaborative filtering, this project identifies movies that are frequently liked together by users and recommends based on those patterns.

## 📌 Dataset

- [MovieLens Dataset](https://grouplens.org/datasets/movielens/) (`ratings.csv`, `movies.csv`)

## 🛠️ Technologies Used

- Python
- Pandas
- mlxtend
- Jupyter Notebook

## 📖 Workflow

1. Load and preprocess the dataset
2. Filter ratings (rating ≥ 4) to treat as "liked" movies
3. Group liked movies per user into transactions
4. Apply `TransactionEncoder` to one-hot encode transactions
5. Generate frequent itemsets using the Apriori algorithm
6. Generate association rules using confidence and lift
7. Recommend movies based on user input

## 💡 Sample Recommendation

**Input:** `Toy Story (1995)`

**Output:**
- Jurassic Park (1993)
- Raiders of the Lost Ark (Indiana Jones and the Raiders of the Lost Ark) (1981)
- Star Wars: Episode V - The Empire Strikes Back (1980)
- Star Wars: Episode IV - A New Hope (1977)
- Indiana Jones and the Last Crusade (1989)

## 📚 What I Learned

- How association rule mining (support, confidence, lift) works in practice
- Using `mlxtend` for frequent itemset mining
- Data preprocessing and transaction encoding with Pandas

## ▶️ How to Run

1. Clone this repository
2. Download `ratings.csv` and `movies.csv` from the [MovieLens dataset](https://grouplens.org/datasets/movielens/) and place them in the project folder
3. Install the required libraries:
   ```bash
   pip install pandas mlxtend
   ```
4. Open and run the Jupyter Notebook
5. Enter a movie name to get recommendations

## 📂 Project Status

✅ Completed

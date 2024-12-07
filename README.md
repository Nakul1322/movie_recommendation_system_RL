
---

# **Movie Recommendation System**

This project implements a **Movie Recommendation System using Reinforcement Learning**. The system leverages user ratings and movie genres to build a personalized recommendation engine that adapts and learns from user interactions over time. The goal is to provide more accurate and dynamic movie recommendations, improving as the system learns from users' preferences.

---

## **Features**
- Load and preprocess movie and ratings data.
- Build and train a recommendation model using deep learning techniques.
- Generate personalized movie recommendations based on user input or preferences.

---

## **Dataset**
The project uses the **MovieLens 25M Dataset**, which is publicly available and can be downloaded from [MovieLens](https://grouplens.org/datasets/movielens/).  

### **Steps to Set Up the Dataset**
1. Download the **MovieLens 25M Dataset** from the official link: [MovieLens 25M Dataset](https://grouplens.org/datasets/movielens/).
2. Unzip the dataset:
   ```bash
   unzip ./ml-25m.zip
   ```
3. Ensure the following files are present in the `ml-25m/` folder:
   - `movies.csv`: Contains movie metadata such as `movieId`, `title`, and `genres`.
   - `ratings.csv`: Includes user ratings with fields like `userId`, `movieId`, `rating`, and `timestamp`.

---

## **Prerequisites**
The following libraries are required to run the project:
- `numpy`
- `pandas`
- `matplotlib`
- `keras`
- `tensorflow`
- `scipy`

---

## **Setup**
1. Clone the repository and ensure the `Data` folder contains the required CSV files.
2. Install the required dependencies using:
   ```bash
   pip install -r requirements.txt
   ```

---

## **How to Use**
1. **Load the Datasets**  
   Start by loading the datasets:
   ```python
   import pandas as pd

   # Load Movies
   movies = pd.read_csv('./Data/movies.csv')
   print(movies.head())

   # Load Ratings
   ratings = pd.read_csv('./Data/ratings.csv')
   print(ratings.head())
   ```

2. **Train the Model**  
   Run the notebook cells or the Python script to train the recommendation model.

3. **Generate Recommendations**  
   Once the model is trained, generate recommendations based on user input or predefined scenarios.

---

## **File Structure**
```
.
├── requirements.txt                  # Dependencies for the project
├── movie_recommendation_system.ipynb  # Jupyter Notebook for model training
└── README.md                         # Project documentation
```

---

## **Future Improvements**
- Enhance recommendation accuracy using hybrid approaches (e.g., combining collaborative filtering with content-based filtering).
- Add a web interface for user interaction.
- Optimize training performance for larger datasets.

---

## **Acknowledgements**
The **MovieLens 25M Dataset** used in this project is publicly available and has been preprocessed to suit the recommendation engine.  
You can access the dataset and more information at [MovieLens 25M Dataset](https://grouplens.org/datasets/movielens/).

---
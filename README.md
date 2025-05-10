# Personalized-News-Recommender-System-using-LightFM-Implicit-Feedback-


This project builds a **hybrid recommendation system** for personalized news using the MovieLens dataset as a proxy. It models **implicit feedback** (treating ratings ≥ 4.0 as positive interactions) and incorporates **content metadata** (genres and tags) to generate **Top-N recommendations** using the LightFM library.

---

Features

* ✅ Models **implicit feedback** (click-like signals)
* ✅ Combines collaborative filtering with content-based features (hybrid model)
* ✅ Trained using **WARP loss** for improved ranking of relevant items
* ✅ Evaluation metrics:
  - `Precision@k`
  - `Recall@k`
  - `AUC` (area under the ROC curve)
  - `Catalog coverage` (diversity of recommendations)
* ✅ Visualizes **Precision–Recall trade-off**
* ✅ Recommends real **movie titles** rather than raw item IDs

---

Results

```text
AUC: 0.9352
Precision@5: 0.4443 | Recall@5: 0.0506
Precision@10: 0.4140 | Recall@10: 0.0891
Precision@20: 0.3628 | Recall@20: 0.1466
Recommendations for user 1: ['Toy Story (1995)', 'Forrest Gump (1994)', 'Jurassic Park (1993)', 'Aladdin (1992)', 'Matrix, The (1999)']
Recommendations for user 2: ['Star Wars: Episode IV - A New Hope (1977)', 'Pulp Fiction (1994)', 'Shawshank Redemption, The (1994)', 'Forrest Gump (1994)', 'Matrix, The (1999)']
Recommendations for user 3: ['Species (1995)', 'Thing, The (1982)', '28 Weeks Later (2007)', 'Planet Terror (2007)', 'Iron Man (2008)']
Recommendations for user 4: ['Shawshank Redemption, The (1994)', "Schindler's List (1993)", 'Graduate, The (1967)', 'American Beauty (1999)', "Amelie (Fabuleux destin d'Amélie Poulain, Le) (2001)"]
Recommendations for user 5: ['Pulp Fiction (1994)', 'Shawshank Redemption, The (1994)', 'Forrest Gump (1994)', "Schindler's List (1993)", 'American Beauty (1999)']
Catalog coverage: 0.27%

```

## Requirements

**Install the necessary Python packages**
pip install lightfm pandas numpy matplotlib
```

```


## How to Run

1. Place the following files in your working directory:

   * `ratings.csv`
   * `movies.csv`
   * `tags.csv`
   * `links.csv`


2. Run the model script


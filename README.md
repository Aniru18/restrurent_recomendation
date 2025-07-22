# 🍽️ Restaurant Recommendation System

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-FA9E32?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 🎯 Objective

To build a **content-based recommendation system** that suggests restaurants to users based on their preferences such as:
- 🍛 Cuisines
- 💰 Price Range
- 🚚 Online Delivery Option
- 🏙️ City

---

## 🧹 Data Preprocessing

- ✅ Removed missing values in key columns: `Cuisines`, `City`, and `Aggregate rating`.
- 🧽 Standardized textual data.
- 🔢 Mapped delivery options like `Yes/No` to numerical values.

---

## 🛠️ Feature Engineering

- **Cuisines**: Vectorized using **TF-IDF** to capture important keywords.
- **Price Range** and **Online Delivery**: Scaled using `StandardScaler` for numerical similarity.
- **City**: One-hot encoded and included in the similarity computation.

---

## 🤖 Recommendation Approach

1. User provides input preferences.
2. The input is transformed into a feature vector.
3. All restaurant records are compared using **cosine similarity**.
4. Results are sorted by **Aggregate Rating** and similarity to return the **Top 5 recommendations**.

---

## 🧑‍💻 User Input Parameters

- `Cuisine`: e.g., `"north indian, chinese"`
- `Price Range`: Integer value from **1 to 4**
- `Online Delivery`: `"Yes"` or `"No"`
- `City`: e.g., `"Delhi"`, `"Bangalore"`

---

## 📤 Output

The system recommends the **Top 5 restaurants** with the following details:

| Field               | Description                     |
|---------------------|---------------------------------|
| Restaurant Name     | Name of the restaurant          |
| City                | City location                   |
| Cuisines            | Cuisine types offered           |
| Price Range         | Cost rating (1: low, 4: high)   |
| Online Delivery     | Whether online delivery is available |
| Aggregate Rating    | Rating score (0–5)              |
| Similarity Score    | Relevance based on input        |

---

## 🧠 Technologies Used

- `pandas`
- `scikit-learn`
- `TF-IDF Vectorizer`
- `Cosine Similarity`

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Aniru18/restaurant_recomendation.git
   cd restaurant_recomendation
# restrurent_recomendation

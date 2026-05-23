# BlueSky – Data Crawling and Analysis

## 📌 Project Description

Connects to BlueSky social media API to collect 250 posts each for keywords: climate, python, and travel. Saves data as JSON files with post text, author info, and engagement stats. Performs text analysis and applies KMeans clustering to discover hidden themes and patterns across posts.

---

## 📂 Project Structure

```
BlueSky-Data-Crawling-and-Analysis/
│
├── 2390829_assignment2_solution.ipynb   # Main Jupyter Notebook
├── 2390829_assignment2_solution.html    # Exported HTML output
├── data/
│   ├── 2390829_climate.json             # 250 posts about "climate"
│   ├── 2390829_python.json              # 250 posts about "python"
│   └── 2390829_travel.json              # 250 posts about "travel"
└── README.md
```

---

## ⚙️ How It Works

### 1. Data Collection
- Connects to the BlueSky API using authentication credentials
- Searches posts using three keywords: **climate**, **python**, and **travel**
- Collects 250 posts per keyword
- Saves each set of posts into a separate JSON file

### 2. Data Storage
Each JSON file stores the following fields for every post:

| Field | Description |
|---|---|
| `text` | Content of the post |
| `author_handle` | Author's username |
| `author_display_name` | Author's display name |
| `like_count` | Number of likes |
| `repost_count` | Number of reposts |
| `reply_count` | Number of replies |
| `quote_count` | Number of quotes |
| `is_reply` | Whether the post is a reply |
| `indexed_at` | Timestamp of the post |
| `uri` | Unique post identifier |

### 3. Text Analysis
- Cleans and processes raw post text
- Removes noise, special characters, and irrelevant content
- Extracts meaningful words and patterns from posts

### 4. KMeans Clustering
- Applies KMeans machine learning algorithm on the collected posts
- Automatically groups similar posts into clusters
- Discovers hidden themes and patterns across different topics without manual labelling

---

## 🛠️ Technologies Used

- **Python 3**
- **atproto** – BlueSky API client
- **scikit-learn** – KMeans Clustering
- **NumPy** – Numerical processing
- **Matplotlib** – Data visualisation
- **JSON** – Data storage

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/BlueSky-Data-Crawling-and-Analysis.git
```

2. Install dependencies:
```bash
pip install atproto scikit-learn numpy matplotlib
```

3. Open the notebook:
```bash
jupyter notebook 2390829_assignment2_solution.ipynb
```

---

## 📊 Keywords Used

| Keyword | Posts Collected |
|---|---|
| climate | 250 |
| python | 250 |
| travel | 250 |
| **Total** | **750** |


# 📊 Data Handling only by using python - Data Science Project

This project is a demonstration of how to build essential data-driven features for a social media platform using only core Python. It includes data loading, cleaning, and recommendation algorithms—implemented without the use of external libraries like Pandas or NumPy.

---

## 📁 Project Structure

```
├── codebook_data.json               # Raw dataset
├── cleaned_codebook_data.json      # Cleaned and structured dataset
├── data_loader.py                  # Script to load and display data
├── data_cleaner.py                 # Script to clean and deduplicate data
├── recommend_friends.py            # People You May Know feature
├── recommend_pages.py              # Pages You Might Like feature

```

---

## 🔍 Overview

This project simulates a social media backend called **CodeBook** with the following objectives:

- Load and display user and page data.
- Clean and structure raw JSON data.
- Recommend friends based on mutual connections.
- Suggest pages based on user interests.

---

## ✅ Features

### 1. Load & Display Data
- Parses JSON file containing users and pages.
- Displays user details including friends and liked pages.

### 2. Data Cleaning
- Handles missing or invalid user names.
- Removes duplicate friend IDs.
- Filters out inactive users.
- Deduplicates pages with conflicting IDs.

### 3. People You May Know
- Suggests users who are not friends but share mutual connections.
- Recommendations ranked by the number of mutual friends.

### 4. Pages You Might Like
- Uses collaborative filtering logic.
- Recommends pages liked by similar users with shared interests.

---

## 🧠 Recommendation Logic

### People You May Know
- A user is suggested if they:
  - Are not already friends.
  - Share one or more mutual friends.

### Pages You Might Like
- Pages are recommended if:
  - They are liked by users with overlapping page interests.
  - Recommendations are scored by the number of shared pages.

---

## 🔧 Tech Stack

- Language: Python 3.x
- Data Format: JSON
- No external libraries used

---

## 🚀 Sample Output

```
Users and Their Connections:
Amit (ID: 1) - Friends: [2, 3] - Liked Pages: [101]
...

Pages:
101: Python Developers
...

People You May Know for User 1: [4]

Pages You Might Like for User 1: [103]
```

---

## 📎 Summary

This project showcases how to simulate real-world data operations on a social network backend using clean and efficient core Python logic. It is ideal for those learning about:

- JSON data processing
- Recommendation algorithms
- Data cleaning workflows
- Pure Python data analysis

---

\

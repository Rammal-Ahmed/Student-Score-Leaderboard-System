# Student Score Leaderboard System
# 🏆 Leaderboard Maker

A small Python project that reads messy lines of student scores, cleans them up, and prints a neat ranked leaderboard.

I built this as part of my Python practice while learning data analytics. The goal was to handle real-world, untidy input instead of perfect data.

---

## What It Does

- Reads lines in the format `Name, score, score, ...`
- Cleans names (removes extra spaces, fixes capitalization)
- Skips empty lines
- Skips entries that have no scores
- Skips entries with invalid scores (for example, `abc`)
- Calculates each person's average, rounded to 1 decimal place
- Ranks everyone from highest average to lowest

---

## Sample Input

```python
lines = [
    "Ayesha, 78, 91, 65",
    "  bilal ,100,80",
    "Chen, 88, 90",
    "Dana",
    "Omar, 85, abc",
    "",
]
```

## Sample Output

```
1. Bilal - 90.0
2. Chen - 89.0
3. Ayesha - 78.0
```

Dana has no scores, Omar has an invalid score, and the blank line is ignored, so none of them appear in the ranking.

---

## How It Works

1. Each line is stripped of extra whitespace.
2. The line is split by commas into a name and a list of scores.
3. The name is cleaned with `.strip().title()`.
4. Every score is checked with `.isdigit()`. One bad score skips the whole line.
5. The average is calculated and stored with the name.
6. The list is sorted, reversed (highest first), and printed with ranks.

---

## Concepts Practiced

- Loops and conditions
- String methods: `strip()`, `split()`, `title()`, `isdigit()`
- Input validation
- Lists and sorting
- Basic data cleaning

---

## How to Run

1. Make sure Python 3 is installed.
2. Clone this repository:
   ```bash
   git clone https://github.com/Rammal-Ahmed/leaderboard-maker.git
   ```
3. Run the file:
   ```bash
   python leaderboard.py
   ```

---

## Possible Improvements

- Read lines from a text or CSV file instead of a hard-coded list
- Accept decimal scores
- Handle ties with a fair shared rank
- Show a short reason for each skipped line

---

## About me

# **Rammal Ahmed**

**AI & Data Science Enthusiast** | **Microsoft Dynamics 365 CRM Developer** | **Power Platform** | **UI/UX Designer** | **Graphic Designer & Illustrator**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rammal-ahmed-58184b325)
[![GitHub](https://img.shields.io/badge/GitHub-Rammal--Ahmed-181717?style=flat&logo=github)](https://github.com/Rammal-Ahmed)

<div align="center">

If you found this useful, consider giving it a star ⭐

**I truly value your feedback and welcome any suggestions for improvement**

**Always open to fresh perspectives, constructive feedback, and new ideas**


## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details

---

*Developed as part of my Python programming practice*

---

**Project Status:** Completed

</div>

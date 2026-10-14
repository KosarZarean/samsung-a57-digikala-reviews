# samsung-a57-digikala-reviews
Sentiment analysis dataset of Samsung Galaxy A57 reviews from Digikala
# Samsung Galaxy A57 Digikala Reviews Dataset

![License](https://img.shields.io/badge/license-CC--BY--4.0-blue)
![Samples](https://img.shields.io/badge/samples-111-green)
![Language](https://img.shields.io/badge/language-Persian-orange)

A Persian-language dataset of customer reviews for the **Samsung Galaxy A57** 
smartphone, collected from [Digikala](https://www.digikala.com/).

Designed for **sentiment analysis** and **text classification** tasks in Persian.

---

## 📊 Dataset Summary

| Feature | Value |
|---|---|
| Total samples | 111 |
| Language | Persian (Farsi) |
| Labels | positive, negative, neutral |
| Source | Digikala |
| Product | Samsung Galaxy A57 (256GB, 8GB RAM) |
| Task | Sentiment Analysis |
| License | CC-BY-4.0 |
| Collection period | 1405/04/02 to 1405/07/22 |

---

## 📈 Label Distribution

| Label | Count | Percentage |
|---|---|---|
| positive | 66 | 59.5% |
| negative | 29 | 26.1% |
| neutral | 16 | 14.4% |
| **Total** | **111** | **100%** |

---

## ✅ Verified Purchase Status

| Status | Count |
|---|---|
| Verified (TRUE) | 92 |
| Not verified (FALSE) | 19 |

---

## 📂 Project Structure

```
samsung-a57-digikala-reviews/
│
├── README.md                 # This file
├── DATASHEET.md              # Full datasheet documentation
├── LICENSE                   # CC-BY-4.0 license
│
└── data/
    ├── clean_comments.csv    # Final cleaned dataset
    └── raw_comments.xlsx     # Raw data
```

---

## 📋 Data Format

| Column | Type | Description |
|---|---|---|
| `id` | integer | Unique identifier |
| `text` | string | Review text (Persian) |
| `label` | string | `positive`, `negative`, or `neutral` |
| `date` | string | Review date (Persian calendar) |
| `verified` | boolean | `TRUE` if verified purchase |

### Example

```csv
id,text,label,date,verified
1,"گوشی خیلی خوبیه، دوربینش عالیه",positive,1405/05/12,TRUE
2,"باتریش زود تموم می‌شه، پشیمون شدم",negative,1405/05/13,TRUE
3,"با A56 فرقش چیه؟",neutral,1405/05/14,FALSE
```

---

## 🚀 Usage

```python
import pandas as pd

df = pd.read_csv('data/clean_comments.csv', encoding='utf-8-sig')

print(df.head())
print(df['label'].value_counts())
print(f"Total samples: {len(df)}")
```

---

## 📖 Documentation

For full details, see [DATASHEET.md](DATASHEET.md).

---

## ⚠️ Limitations

- This dataset covers only one specific product (Samsung Galaxy A57).
- Some reviews may be fake or promotional.
- Labeling was done by one person and may be subjective.
- The dataset is not balanced (59.5% positive).
- Some reviews complain about price or logistics, not the product itself.

---

## 📜 License

This dataset is licensed under the 
[Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

---

## 📝 Citation

> Zarean, K. (2026). *Samsung Galaxy A57 Digikala Reviews Dataset*. 
> GitHub. https://github.com/KosarZarean/samsung-a57-digikala-reviews

---

## 📧 Contact

**Author:** Kousar Zarean  
**Email:** kzaran79@gmail.com  
**GitHub:** [@KosarZarean](https://github.com/KosarZarean)

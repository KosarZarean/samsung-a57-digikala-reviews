# Datasheet for Samsung Galaxy A57 Digikala Reviews Dataset

**Version:** 1.0  
**Date:** 2026-10-14  
**Author:** Kousar Zarean  
**Repository:** https://github.com/KosarZarean/samsung-a57-digikala-reviews

---

## Motivation

**For what purpose was the dataset created?**

This dataset was created for the **Trustworthy Machine Learning** course 
project, with the goal of analyzing the sentiment of customer reviews for 
the Samsung Galaxy A57 smartphone. The main objective is to provide a labeled 
Persian-language dataset for training text classification and sentiment 
analysis models.

**Who created the dataset?**

Kousar Zarean, Shahrekord University, Trustworthy Machine Learning, 
Instructor: Dr. Basiri

**Who funded the creation of the dataset?**

Course project, no external funding.

**Any other comments?**

Selected product: Samsung Galaxy A57 Dual SIM, 256GB storage, 8GB RAM, 
Vietnam region. Product link on Digikala:  
https://www.digikala.com/product/dkp-21660239/

---

## Composition

**What do the instances represent?**

Each instance is a textual review from buyers of the Galaxy A57 smartphone 
on Digikala. Each instance contains the review text, sentiment label 
(positive/negative/neutral), date, and verified purchase status.

**How many instances are there?**

111 reviews, including:
- 66 positive
- 29 negative
- 16 neutral

**Is this a sample or the complete set?**

No, it is a sample of the 251 reviews available on the product page.  
Sampling strategy: all reviews with 15+ characters.  
Representativeness: the rating distribution of this dataset was compared 
with the overall distribution (average 4.4 from 336 buyers).

**What data does each instance consist of?**

Text + label + date + verified purchase status (no usernames).

**Is there a label or target?**

Yes: positive / negative / neutral

**Is any information missing?**

Usernames and personal information have been removed for privacy reasons.

**Are relationships between instances explicit?**

No.

**Are there recommended data splits?**

No. The dataset is provided as a single file.

**Are there errors, noise, or redundancies?**

Duplicate reviews were removed. There is a possibility of fake 
(promotional) reviews.

**Is the dataset self-contained?**

Yes, entirely in the CSV file.

**Does it contain confidential data?**

No, reviews were public and have been anonymized.

**Does it contain offensive content?**

Some reviews may be sarcastic or critical.

**Subpopulations?**

Demographic information is not available from Digikala.

**Can individuals be identified?**

No, names and personal information have been removed.

**Sensitive data?**

No.

---

## Collection Process

**How was the data acquired?**

Directly extracted from the Digikala product page (link above) manually.

**Mechanisms or procedures?**

Google Chrome browser + Microsoft Excel.

**Sampling strategy?**

All reviews with 15+ characters.

**Who was involved?**

Kousar Zarean alone.

**Over what timeframe?**

Reviews were written from 1405/04/02 to 1405/07/22.  
Collection was performed on 1405/07/25.

**Ethical review?**

No, course project.

**Were individuals notified?**

No, reviews were publicly posted.

**Did individuals consent?**

Reviews are public, but explicit consent was not obtained.

**Revoke mechanism?**

If a review is removed from Digikala, it will be removed from the dataset.

**Impact analysis?**

No.

---

## Preprocessing/Cleaning/Labeling

**Was any preprocessing done?**

Yes:
- Removal of usernames and personal information
- Removal of duplicate reviews
- Removal of reviews under 15 characters

**Was raw data saved?**

Yes, in `data/raw_comments.xlsx`

**Software used?**

Microsoft Excel (manual)

**Labeling guidelines?**

- **positive:** praise of the product, satisfaction with purchase, 
  recommendation to others
- **negative:** criticism of the product, dissatisfaction, price complaints, 
  logistics issues
- **neutral:** questions, information sharing, comparison without judgment

---

## Uses

**Has the dataset been used?**

Yes, for the Trustworthy Machine Learning course project.

**Repository of papers?**

https://github.com/KosarZarean/samsung-a57-digikala-reviews

**What tasks could it be used for?**

- Persian sentiment analysis
- Training text classification models
- Analyzing reviews of similar products

**Anything impacting future uses?**

- Some reviews may be fake.
- It is about only one specific product.
- Generalization to other products requires caution.

**Tasks it should NOT be used for?**

- Judging the overall quality of the Samsung brand
- Detecting fake reviews (no fake label available)
- Analyzing other products without retraining

---

## Distribution

**Will it be distributed?**

Yes, on GitHub.

**How?**

GitHub repo + CSV file + README + DATASHEET.md

**DOI?**

N/A

**When?**

2026-10-14

**License?**

CC-BY-4.0

**Third-party restrictions?**

No.

**Export controls?**

No.

---

## Maintenance

**Who maintains it?**

Kousar Zarean

**Contact?**

kzaran79@gmail.com

**Erratum?**

In GitHub Issues

**Will it be updated?**

No

**Retention limits?**

If a review is removed from Digikala, it will be removed from the dataset.

**Older versions?**

No

**Contribution mechanism?**

GitHub Pull Request

---

## Limitations

- This dataset only covers reviews of one specific product (Galaxy A57).
- Some reviews may have been written by sellers or competitors (fake reviews).
- Digikala reviews may be affected by display algorithms.
- Labeling was done by one person and may be subjective.
- The datasheet cannot guarantee the absence of bias.
- Class distribution is imbalanced: 59.5% positive, 26.1% negative, 14.4% neutral.
- A frequent pattern: complaints about **high price** or **price fluctuation** 
  (about 20% of reviews).
- Some reviews contain complaints about **logistics, shipping, registration, 
  or packaging**, not about the product itself.

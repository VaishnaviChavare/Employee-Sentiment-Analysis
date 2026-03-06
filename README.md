# Employee-Sentiment-Analysis

## Summary:
Analyzed 2,191 historical Enron emails (2010–2011) from 10 key employees

Combined subject + body → applied transformer-based sentiment classification

Initial model showed 100% Positive bias → switched to balanced model → ~72% Neutral, ~22% Positive, ~6% Negative

Created monthly sentiment scores (+1 / 0 / –1) and ranked employees (top positive & most negative per month)

Implemented rolling 30-day flight-risk detection (≥4 negative emails) → no triggers found

Built binary classification models (Logistic Regression + Random Forest) to predict negative-sentiment emails
→ Useful signals: keyword presence, reply status, message length, sender activity

Key insight: Formal business emails rarely show explicit negativity → hybrid (model + rules) approach recommended

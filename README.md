# Customer-Churn-Analysis-and-Insights
A churn analysis project for a B2B international payments platform, uncovering customer retention patterns and behavioral drivers using Python, Power BI, and transactional data. Includes strategic recommendations for improving customer lifetime value through tailored retention and reactivation strategies.

## 📌 Goal
To uncover key behavioral drivers of customer churn and develop actionable, retention-focused marketing strategies tailored to B2B money transfer platform.

### Sub-Questions Explored:
- What is the churn rate, and how should churn be defined?
- What behavioral patterns (e.g. frequency, spend, value) distinguish churned from retained customers?
- How does churn differ by industry or transaction size?
- Which segments offer the most retention potential or LTV?

---

## 📂 Files Included

| File | Description |
|------|-------------|
| `churn_analysis.ipynb` | Python notebook with data prep, feature engineering, EDA |
| `Churn_Analysis_Visualisation.pbix` | Power BI dashboard with churn segmentation |
| `Methodologies and Findings Report.pdf` | Full methodology, analysis, and strategic recommendations |

## 🧪 Methodology

### ✅ Defining Churn
- Churn is defined as **no transaction within the past 90 days before Dec 30, 2022**.
- Churn segments:
  - **Recent (<1 year)** — reactivation potential
  - **Dormant (1–5 years)** — harder to win back
  - **Historical (>5 years)** — excluded as likely lost

### 🧠 Feature Engineering
Key features created:
- First and last transaction dates
- Transaction count
- Total and average spend
- Industry type

---

## 📊 Exploratory Analysis

### 🔸 Overall Churn Rate
- **93.5%** of users churned — indicating a serious retention challenge.

### 🔸 Lifetime Patterns
![image](https://github.com/user-attachments/assets/929bf775-a8ed-4058-9f01-7a97c6f7c34c)

The purpose of this graph is to visually compare the customer lifetime between churned and retained users and to understand how long customers typically stay before they churn ad if retained users behave differently.

- Retained users had **longer lifetimes (~559 days)** vs. churned (~387 days).
- Early drop-off is common — many churn within **30–60 days** of joining.

' A critical opportunity if we can engage users earlier and extend their time on the platform beyond this valuable window, so we can significantly reduce churn'.

### 🔸 Frequency vs Spend
![image](https://github.com/user-attachments/assets/2a3c7c17-7799-4784-8eec-fb5aec544d94)
- Retained users transacted more frequently (~67 vs ~47 median transactions)

![image](https://github.com/user-attachments/assets/185ead3a-8353-4f2a-b0f6-ede6146b93ea)
- Total spend is higher for retained users (£32k vs £23.7k), but:
  > Some churned users spent a lot once and left — **big spend ≠ loyalty**.


### 🔸 Transaction Amount Patterns
![image](https://github.com/user-attachments/assets/f6911902-255e-48f9-af37-2ee706bfff2b)
- Most loyal users transacted **consistently in the £100–£999** range.
- One-off high-value users (e.g. £1,000+) showed **high churn risk**.

### 🔸 Industry Patterns
- **Finance & Healthcare:** High spend but 100% churn.
- **Technology & Retail:** Longer lifetimes, better LTV, but still churn-prone.
- **Crypto & Manufacturing:** Better retention, but lower value.
- Insight: **Industry-specific behavior requires tailored strategies**.

---

## 📈 Power BI Dashboard Highlights
- Visualizes churn by:
- User lifetime and transaction frequency
<img width="602" alt="image" src="https://github.com/user-attachments/assets/38d4dfd9-c01f-4355-b963-51790d8a8af9" />

- Spend brackets
- Industry segment
'Supports decision-making for targeted retention strategies'
<img width="603" alt="image" src="https://github.com/user-attachments/assets/0ed73aa7-65dc-4061-91fb-8a87b1b348ad" />


---

## 💡 Strategic Recommendations

### 🎯 Retention
#### Objective: Boost long-term retention and repeat usage among business customers to increase LTV.
1. **Lifecycle-Driven Engagement** – Target users by stage (onboarding → mid-lifecycle).
2. **Scheduled Transfer Nudges** – Build habits with recurring reminders.
3. **Tailored Onboarding by Industry** – Customized activation paths.
4. **Loyalty Rewards** – Encourage consistent usage through milestone perks.
5. **Feature Discovery Campaigns** – Educate users on underused tools (e.g., batch transfers).

### 🔁 Reactivation
#### Objective: Re-engage dormant users and drive renewed transfer activity
1. **Win-Back Campaigns** – Personalized offers for lapsed high-value users.
2. **Time-Limited FX Discounts** – Drive urgency to reactivate.
3. **Referral Incentives** – Reward returning users who invite others.
4. **Exit Surveys & Retargeting** – Capture feedback to tailor campaigns.
5. **Frictionless Return Path** – Simplify re-entry with saved data & one-click login.

---

## 📊 Key Takeaways

- **Churn = activation + retention problem** — many users drop off early.
- **High spend ≠ high loyalty** — repeat usage matters more.
- **Segmented strategies outperform generic ones** — especially by industry.
- Wise must support users in forming habits, not just delivering a good first experience.

---

## 🛠️ Tech Stack
- Python (pandas, matplotlib, seaborn)
- Power BI
- Jupyter Notebook
- Excel

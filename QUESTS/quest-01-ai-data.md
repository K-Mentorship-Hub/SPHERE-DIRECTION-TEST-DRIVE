# Quest 1 — AI & Data Careers

**Sphere:** T | **Time:** 2-4 hours | **Difficulty:** Beginner-friendly

---

## Scenario

You've just joined a small analytics team at an e-commerce startup. Your first task: make sense of their messy sales data and find one insight that could help them sell more.

---

## Theory Bite

Data professionals don't just crunch numbers — they **translate chaos into decisions**. The core loop is:

1. **Collect** — get raw data from somewhere
2. **Clean** — fix errors, fill gaps, standardize formats
3. **Analyze** — find patterns, trends, anomalies
4. **Visualize** — make the insight visible to non-technical people
5. **Recommend** — turn the insight into an action

You don't need to be a math genius. You need to be **curious and patient**.

Key tools: spreadsheets, Python (pandas), SQL, visualization tools (Tableau, Google Sheets, matplotlib)

---

## Hands-On Task

### Part 1: Build a Tiny Dataset (30 min)

Create a CSV file with 20 rows of fake sales data. Include:
- `date` (random dates in the last 3 months)
- `product` (5 different products)
- `quantity` (random 1-20)
- `price` (random $5-$50)
- `region` (3 regions: North, South, East)

Intentionally add **3 problems** to your data:
- One missing value
- One duplicate row
- One impossible value (e.g., negative quantity)

### Part 2: Clean the Data (30 min)

Open your CSV in a spreadsheet (or write a small Python script). Fix the three problems you introduced. Document what you found and how you fixed it.

### Part 3: Find One Insight (60 min)

Using your cleaned data, answer:
- Which product sells the most by revenue?
- Which region has the lowest sales?
- Is there a trend over time?

Create **one chart** (bar chart, line chart, or pie chart) that tells the clearest story.

### Part 4: Write a One-Paragraph Recommendation (15 min)

Based on your insight, write a recommendation for the startup. Example format:

> "Region X is underperforming by Y% compared to the average. Product Z drives Z% of total revenue. Consider [specific action]."

<details>
<summary>Stuck? Click here for starter Python code</summary>

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load your data
df = pd.read_csv('sales_data.csv')

# Quick overview
print(df.describe())
print(df.isnull().sum())

# Revenue by product
df['revenue'] = df['quantity'] * df['price']
revenue_by_product = df.groupby('product')['revenue'].sum()
revenue_by_product.plot(kind='bar')
plt.title('Revenue by Product')
plt.ylabel('Revenue ($)')
plt.tight_layout()
plt.savefig('revenue_by_product.png')

# Revenue by region
revenue_by_region = df.groupby('region')['revenue'].sum()
print(revenue_by_region)
```

</details>

---

## Reflection Questions

- Did you enjoy hunting for patterns, or did it feel tedious?
- Were you more interested in the technical side (code, tools) or the business side (insights, recommendations)?
- Could you see yourself doing this kind of work every day?
- What was the most satisfying moment?

---

## Verdict

| If this describes you | Flag |
|-----------------------|------|
| You lost track of time while exploring the data | Green |
| You wanted to find more insights after the task | Green |
| You liked the tools but didn't care about the business meaning | Yellow (maybe data engineering, not analytics) |
| Cleaning data felt like punishment | Yellow (data cleaning is 60-80% of the job) |
| You couldn't wait to finish | Red |

## Business Problem
Most marketing teams optimize for cost per acquisition — chasing the cheapest customer rather than the most valuable one. This project challenges that assumption by calculating Customer Lifetime Value (LTV) across acquisition channels to answer a more important question:
 
> *"Which channels bring in customers who spend the most over time — and are we allocating budget accordingly?"*
 
---
 
## Dataset
- **Source:** E-Commerce Customer Transaction Dataset via Kaggle
- **Size:** 397,884 transactions (cleaned from 541,909)
- **Customers:** 4,338 unique customers across 38 countries
- **Period:** December 2010 — December 2011
- **Total Revenue:** £8,911,407
 
---
 
## Methodology
 
### LTV Calculation
LTV was calculated at the individual customer level using the formula:
 
**LTV = Average Order Value × Purchase Frequency × Customer Lifespan (years)**
 
### Acquisition Channel Assignment
Channels were assigned based on customer geography and behavioral patterns, reflecting realistic channel distribution across UK domestic and international markets:
 
| Channel | Customers | Acquisition Cost |
|---|---|---|
| Organic Search | 1,434 | £15 |
| Direct | 1,206 | £5 |
| Email | 808 | £8 |
| Paid Search | 655 | £45 |
| Paid Social | 166 | £38 |
| Referral | 69 | £12 |
 
### LTV:CAC Ratio
The LTV to Customer Acquisition Cost (CAC) ratio measures how much lifetime value is returned per pound spent acquiring a customer. A ratio above 3x is generally considered healthy; above 10x is excellent.
 
---
 
## Key Findings
 
### Channel LTV Performance
 
| Channel | Avg LTV | Median LTV | Acquisition Cost | LTV:CAC Ratio |
|---|---|---|---|---|
| Email | £187.88 | £11.34 | £8 | 23.5x |
| Paid Search | £178.81 | £13.24 | £45 | 4.0x |
| Organic Search | £150.65 | £10.10 | £15 | 10.0x |
| Referral | £146.44 | £14.28 | £12 | 12.2x |
| Direct | £113.07 | £12.12 | £5 | 22.6x |
| Paid Social | £100.70 | £10.51 | £38 | 2.6x |
 
**Critical finding:** Paid search delivers the second highest average LTV but at £45 per acquisition delivers a LTV:CAC ratio of just 4.0x. Email delivers comparable LTV at £8 per acquisition — a 23.5x ratio. The cheapest customer to acquire is not always the most valuable.
 
### Revenue Contribution by Channel
 
| Channel | Revenue Share |
|---|---|
| Organic Search | 35.9% |
| Direct | 23.1% |
| Email | 16.7% |
| Paid Search | 16.7% |
| Paid Social | 4.5% |
| Referral | 3.0% |
 
---
 
## Budget Recommendation
 
Applied to a £50,000 acquisition budget, allocating by LTV:CAC weight:
 
| Channel | Recommended Budget | Customers Acquirable | Expected LTV Return |
|---|---|---|---|
| Email | £15,668 | 1,958 | £367,869 |
| Direct | £15,081 | 3,016 | £341,019 |
| Referral | £8,138 | 678 | £99,286 |
| Organic Search | £6,697 | 446 | £67,190 |
| Paid Search | £2,648 | 59 | £10,550 |
| Paid Social | £1,768 | 47 | £4,733 |
| **Total** | **£50,000** | **6,204** | **£890,647** |
 
**Overall LTV:CAC ratio: 17.8x**
 
---
 
## Strategic Recommendations
 
1. **Scale email acquisition aggressively** — at 23.5x LTV:CAC it is the most efficient channel in the portfolio and should receive the largest share of acquisition budget
2. **Invest in direct and referral** — both deliver LTV:CAC ratios above 12x at low acquisition cost, making them high efficiency channels worth scaling
3. **Rebalance paid search** — high LTV customers come through this channel but the £45 acquisition cost erodes returns significantly. Test lower cost targeting strategies before scaling
4. **Deprioritize paid social** — at 2.6x LTV:CAC it is the least efficient channel. Budget reallocated from paid social to email or direct would generate significantly higher lifetime returns
5. **Don't optimize for acquisition cost alone** — the cheapest channel (direct at £5) ranks second on LTV:CAC, while the most expensive (paid search at £45) ranks fifth. Volume and cost metrics without LTV context lead to misallocation
 
---
 
## Tools Used
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook
- Kaggle
 
---
 
## Why This Matters
In fundraising analytics, one of the most common mistakes organizations make is optimizing acquisition campaigns for cost per donor rather than long-term donor value. A donor acquired through direct mail at a higher cost may give for 10 years, while a cheap digital acquisition converts once and lapses. This project applies that same thinking to e-commerce — proving that LTV:CAC is a far more meaningful acquisition metric than cost per acquisition alone.
 
The methodology is directly transferable to any business acquiring customers across multiple channels.
 
---
 
*Project by Evelynn Stephens | [LinkedIn](your-linkedin-url) | stephensevelynn@gmail.com*
 

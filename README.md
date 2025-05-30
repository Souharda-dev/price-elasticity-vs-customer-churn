Project Overview
The client wants to understand how changes in service pricing affect customer churn (customers leaving for competitors). This project uses machine learning to:

Predict churn probability based on pricing and customer behavior.

Analyze price sensitivity across different customer segments.

Recommend pricing strategies to minimize churn while maximizing revenue.

Methodology
Dataset: Synthetic customer data (tenure, monthly charges, price changes, contract type, etc.).

Techniques:

SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalance (few churn cases).

Random Forest Classifier for robust predictions.

Feature Importance Analysis to identify key drivers of churn.

Price Sensitivity Simulation to test how different pricing affects churn.

Key Insights from Analysis
1. Churn Distribution & Class Imbalance
Original dataset had 15% churn (imbalanced) → SMOTE balanced it for better model training.

High churn risk when:

Price increases (especially for monthly contract customers).

Low tenure (new customers more likely to leave).

High customer service calls (indicates dissatisfaction).

2. Impact of Price Changes on Churn
Price increases (+5%) → ↑ 20-30% churn probability for monthly contract customers.

Price decreases (-5%) → ↓ 10-15% churn probability, but revenue impact must be considered.

Annual contract customers are less sensitive to price changes (stickier customers).

3. Most Important Features Driving Churn
Feature	Impact on Churn
Price Change %	Highest impact – increases churn when prices rise.
Monthly Charge	Higher bills → higher churn risk.
Tenure	New customers churn more than long-term ones.
Contract Type (Monthly)	Monthly customers are most price-sensitive.
Customer Service Calls	More calls → higher dissatisfaction → churn.
4. Segment-Specific Findings
Customer Segment	Churn Risk	Price Sensitivity
Monthly Contract	High	Very sensitive
Annual Contract	Medium	Moderately sensitive
High Usage Customers	Medium-High	Sensitive to price hikes
Low Tenure (<1 year)	High	Highly sensitive
Strategic Recommendations for British Gas
1. Dynamic Pricing Strategies
✅ For Monthly Contract Customers

Avoid sudden price increases → High churn risk.

Offer incentives (e.g., loyalty discounts) to retain them.

Upsell to annual contracts (lower churn, more stable revenue).

✅ For Annual Contract Customers

More flexibility with pricing (less churn risk).

Small price increases (2-3%) can be tested with minimal churn impact.

✅ For High-Usage Customers

Volume discounts to retain them (high-value segment).

Personalized offers to prevent switching to competitors.

2. Retention Tactics for At-Risk Customers
🔹 Identify high-churn-risk customers:

New customers (<6 months tenure) → Offer welcome discounts.

Customers with recent price hikes → Proactively reach out with retention offers.

Frequent service callers → Investigate pain points (billing issues, service quality).

🔹 Personalized Retention Offers:

Discounts for long-term commitments (e.g., switch to 2-year contract).

Bundle deals (e.g., free smart thermostat with renewal).

3. A/B Testing for Pricing Changes
Test small price adjustments (1-5%) in controlled groups.

Monitor churn impact before rolling out changes company-wide.

4. Proactive Churn Prevention
Early warning system: Use ML model to flag high-risk accounts.

Customer feedback loops: Survey customers after price changes.

Competitor price benchmarking: Ensure British Gas remains competitive.


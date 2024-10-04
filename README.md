# 🎮 Mobile Games A/B Testing: Cookie Cats Gate Placement

## 📝 Objective
Analyze how gate placement (level 30 vs. level 40) in the mobile game **Cookie Cats** impacts player retention. The A/B test aims to determine whether moving the gate influences 1-day and 7-day retention rates, providing insights for improving player engagement.

## ❓ Key Questions
- Does gate placement affect player retention?
- How do retention rates differ between the two groups?
- Can we be confident in these differences through statistical testing?

## 📊 Data
The dataset consists of 90,189 players who installed the game during the test. Key columns:
- `userid`: Unique player identifier
- `version`: Group (gate_30 or gate_40)
- `sum_gamerounds`: Number of rounds played in the first 14 days
- `retention_1`: Did the player return 1 day after installation?
- `retention_7`: Did the player return 7 days after installation?

## 🧠 Approach
1. **Data Exploration**: Analyzed player distribution and gameplay behavior.
2. **Group Comparison**: Assessed differences in retention between gate_30 and gate_40 groups.
3. **Statistical Analysis**: Used bootstrapping to determine the significance of differences.

## 📈 Results
- **1-day retention**: Slightly lower in gate_40 (44.2%) compared to gate_30 (44.8%).
- **7-day retention**: Decreased from 19.0% (gate_30) to 18.2% (gate_40).
- Bootstrapping shows 96.6% probability that gate_30 has higher 1-day retention, and 100% certainty for 7-day retention.

## 🚀 Conclusion
Keeping the gate at level 30 improves player retention. The results suggest a significant drop in both 1-day and 7-day retention when the gate is moved to level 40, making the earlier gate placement more effective.

## 🛠️ Tools & Libraries
- **pandas**: Data analysis and manipulation
- **matplotlib**, **seaborn**, **plotly**: Data visualization
- **SciPy**: Statistical analysis


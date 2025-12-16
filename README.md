# The-Evolution-of-Success-on-Kickstarter
Analysis of Kickstarter campaigns using data science to identify structural drivers of crowdfunding success, assess predictive performance, temporal evolution, and the platform’s maturation.

Crowdfunding platforms such as Kickstarter have grown into major funding ecosystems, yet most projects still fail.
Understanding which structural factors drive campaign success, and how these patterns evolve over time, is essential for reducing risk and improving decision-making by creators and investors.
Data-driven approaches offer a systematic way to uncover these patterns and build predictive insights at scale.

### Dataset
- Source: Kickstarter public dataset (via WebRobots)
- Period: 2009-2024
- Campaigns: 411,640
- Target variable: campaign success (binary). Defined by reaching monetary goal by end of determined duration.
- Features:
  - Financial (goal, pledged, backers)
  - Temporal (campaign duration, launch year)
  - Creator reputation (past projects, past success)
  - Categorical (project category)
 
### Methodology
1. Exploratory data analysis to identify temporal and structural patterns
2. Feature engineering (log transforms, categorical encoding, reputation metric contruction)
3. Supervised learning with LightGBM
4. Model evaluation using ROC-AUC
5. Temporal validation using yearly data splits
6. In-depth analysis of features

### Key Results
- Overall model performance using full dataset: ROC-AUC = 0.80
- Progressive improvement in predictive performance over time using datasets stratified by year
- Significant structural drivers of success:
  - Financial goal
  - Campaign duration
  - Creator reputation
  - Project category

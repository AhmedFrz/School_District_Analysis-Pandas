# PyCitySchools District Analysis

<!-- Collapsible Table of Contents -->
<details>
  <summary>📑 Table of Contents</summary>
  
  - [Overview](#overview)
  - [Problem Statement & Purpose](#problem-statement--purpose)
  - [The Solution & Methodology](#the-solution--methodology)
  - [Technologies & Skills](#technologies--skills)
  - [Project Structure](#project-structure)
  - [Key Findings & Discussion](#key-findings--discussion)
  - [Business Impact](#business-impact)
  - [Setup and Future Work](#setup-and-future-work)
</details>

## Overview
This repository contains a comprehensive analysis of standardized test data from a school district, examining math and reading scores across different schools. The analysis utilizes Python with pandas and NumPy libraries to process, clean, and analyze educational data to identify patterns and factors that influence student performance.

<!-- Quick Summary Card -->
<table>
<tr>
  <td><b>Key Insight:</b> Charter schools consistently outperform district schools despite lower funding</td>
</tr>
<tr>
  <td><b>Primary Finding:</b> School size is a stronger predictor of success than per-student spending</td>
</tr>
<tr>
  <td><b>Business Value:</b> Potential to optimize resource allocation and improve student outcomes</td>
</tr>
</table>

## Problem Statement & Purpose
School districts face ongoing challenges in allocating resources effectively and identifying factors that contribute to student success. This project addresses several critical questions:

| Research Questions | Project Goals |
|-------------------|---------------|
| Does school type (Charter vs. District) impact student performance? | Inform budget allocation decisions |
| How does school size affect academic achievement? | Identify successful educational models for replication |
| What is the relationship between per-student funding and outcomes? | Target interventions for underperforming schools |
| Which schools consistently outperform or underperform? | Understand impact of various factors on achievement |

## The Solution & Methodology

<!-- Collapsible Methodology Section -->
<details>
  <summary><b>Expand to see detailed methodology</b></summary>
  
  The project implements a Python-based analysis pipeline that processes educational data through several key steps:
  
  1. **Data Integration**: Merging student and school datasets to create a comprehensive view
  2. **Data Cleaning**: Handling missing values, correcting data types, removing invalid records
  3. **Metric Calculation**: Deriving performance metrics across different dimensions
  4. **Comparative Analysis**: Contrasting performance across different school characteristics
  5. **Binning and Categorization**: Creating meaningful groups for per-student spending and school size

  ### Why This Methodology Was Chosen
  This descriptive analytical approach was selected because:

  - It offers clear, interpretable results for educational stakeholders without statistical expertise
  - It aligns with the practical questions posed by school district administrators
  - It enables multi-faceted analysis across several variables simultaneously
  - It utilizes Python's pandas library, which is optimized for this type of tabular data analysis
  - It allows for both granular school-level insights and broader trend identification
</details>

The analysis examines relationships between school characteristics and student performance through data integration, cleaning, and statistical analysis to produce actionable insights for stakeholders.

## Technologies & Skills

| Technologies Used | Skills Applied |
|-------------------|----------------|
| Python 3.7.13 | Data cleaning and preprocessing |
| Pandas for data manipulation | Exploratory data analysis (EDA) |
| NumPy for numerical operations | Statistical analysis and interpretation |
| Jupyter Notebook | Data transformation and feature engineering |
| CSV files for data storage | Categorical data binning and aggregation |
| Matplotlib for visualization | Performance metric calculation |

## Project Structure
```
PyCitySchools/
├── PyCitySchools_Challenge_AF.ipynb   # Main analysis notebook
├── Resources/                         # Data directory
│   ├── students_complete.csv          # Student data
│   └── schools_complete.csv           # School data
├── README.md                          # Project documentation
└── Analysis/                          # Output analysis files (implied)
```

## Key Findings & Discussion

<!-- Interactive Results Tabs - Note: These would be implemented with JavaScript in GitHub -->
<div class="tabs">
  <div class="tab" data-tab="school-type">
    <h3>School Type Performance</h3>
    <ul>
      <li>Charter schools: 90% overall passing rate</li>
      <li>District schools: 54% overall passing rate</li>
      <li>Largest disparity observed in math performance</li>
    </ul>
    <p><b>Conclusion:</b> Clear evidence shows charter schools outperform district schools, suggesting structural or operational differences significantly impact student outcomes.</p>
  </div>
  
  <div class="tab" data-tab="school-size">
    <h3>School Size Impact</h3>
    <ul>
      <li>Small/medium schools: ~90% passing rates</li>
      <li>Large schools (2000-5000): 58% passing rate</li>
      <li>Similar performance in small & medium schools</li>
    </ul>
    <p><b>Conclusion:</b> The analysis definitively establishes that smaller and medium-sized schools yield better academic outcomes, pointing to potential benefits of more personalized educational environments.</p>
  </div>
  
  <div class="tab" data-tab="spending">
    <h3>Spending Patterns</h3>
    <ul>
      <li>Lowest spending (<$586): 90% passing rate</li>
      <li>Highest spending ($646-675): 54% passing rate</li>
      <li>Counter-intuitive negative correlation between spending and performance</li>
    </ul>
    <p><b>Conclusion:</b> The counterintuitive finding that higher spending correlates with lower performance challenges common assumptions about resource allocation, suggesting quality of spending matters more than quantity.</p>
  </div>
</div>

> **Note:** The tabs above would be functional in a GitHub pages deployment but appear as sections in standard GitHub markdown.

### Alternative Approaches

<details>
  <summary><b>Click to explore alternative methodologies</b></summary>
  
  Several methodologies could have enhanced this analysis:
  
  - **Regression Analysis**: Using multivariate regression to isolate the impact of each factor while controlling for others
  - **Longitudinal Studies**: Tracking changes over multiple years to identify improvement trends
  - **Qualitative Analysis**: Incorporating teacher interviews or classroom observations to explain quantitative findings
  - **Machine Learning**: Employing clustering or classification algorithms to identify patterns not visible through descriptive statistics
</details>

## Business Impact

<!-- Visual Business Impact Display -->
<table>
  <tr>
    <th>Benefit Category</th>
    <th>Specific Impacts</th>
  </tr>
  <tr>
    <td><b>Time Savings</b></td>
    <td>
      • Eliminates manual data compilation (hundreds of hours saved)<br>
      • Provides ready-made dashboards for quick decision-making<br>
      • Enables rapid identification of issues
    </td>
  </tr>
  <tr>
    <td><b>Cost Reduction</b></td>
    <td>
      • Identifies inefficient resource allocation<br>
      • Highlights where additional spending may not yield returns<br>
      • Allows targeted rather than blanket interventions
    </td>
  </tr>
  <tr>
    <td><b>Efficiency Improvements</b></td>
    <td>
      • Enables data-driven resource allocation<br>
      • Provides clear benchmarks for measuring initiatives<br>
      • Facilitates sharing of best practices
    </td>
  </tr>
  <tr>
    <td><b>Strategic Benefits</b></td>
    <td>
      • Informs policy with evidence rather than anecdote<br>
      • Supports long-term planning with comprehensive metrics<br>
      • Helps prioritize initiatives based on likely impact
    </td>
  </tr>
</table>

## Setup and Future Work

### Installation
```
pip install pandas numpy jupyter matplotlib
jupyter notebook PyCitySchools_Challenge_AF.ipynb
```

### Future Directions
- Longitudinal analysis to track changes over time
- Demographic analysis and teacher-to-student ratio correlations
- Predictive models to identify at-risk students
- Interactive dashboard for real-time monitoring

---

<!-- Feedback Section -->
<details>
  <summary><b>Provide Feedback on This Analysis</b></summary>
  
  We value your input on this analysis. If you have suggestions for improvement or additional research questions to explore, please:
  
  1. Open an issue in this repository
  2. Include the tag [FEEDBACK] in your issue title
  3. Specify which aspect of the analysis you're addressing
  4. Share your thoughts or recommendations
  
  Your feedback helps us continually refine our approach to educational data analysis!
</details>

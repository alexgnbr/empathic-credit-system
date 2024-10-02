# CloudWalk Technical Case: The Empathic Credit System (ECS)

## Background
CloudWalk has developed a groundbreaking Empathic Credit System (ECS) that uses real-time emotional and contextual data to offer personalized credit to users. This system has been integrated into CloudWalk's mobile app and has collected data from millions of customers. As a Data Analyst, your task is to analyze this rich dataset, extract meaningful insights, and provide recommendations to improve the system's effectiveness and fairness.

## The Data Analysis Challenge

### Dataset Overview
You have access to a SQLite database (`ecs_data.db`) containing the following tables:

## Table: users

| Column | Type |
|--------|------|
| user_id | TEXT |

## Table: emotional_data

| Column | Type |
|--------|------|
| user_id | TEXT |
| timestamp | TIMESTAMP |
| intensity | REAL |
| time_of_day | TEXT |
| primary_emotion | TEXT |
| relationship | TEXT |
| relationship_closeness | INTEGER |
| situation | TEXT |
| location | TEXT |
| weather | TEXT |
| physical_state | TEXT |
| preceding_event | TEXT |

## Table: loans

| Column | Type |
|--------|------|
| loan_id | INTEGER |
| user_id | TEXT |
| loan_amount | INTEGER |
| issue_date | TIMESTAMP |
| due_date | TIMESTAMP |
| loan_term | INTEGER |
| status | TEXT |
| paid_date | TIMESTAMP |
| interest_rate | REAL |
| total_amount | REAL |
| installment_amount | REAL |
| loan_amount_paid | REAL |

### Task Requirements

1. Data Exploration and Preprocessing:
   - Connect to the SQLite database and perform initial data exploration.
   - Handle any data quality issues.

2. Emotional Pattern Analysis:
   - Identify dominant emotional patterns for users over time.
   - Analyze how emotions correlate with different contexts (e.g., relationships, situations, time of day).

3. Loan-Emotion Correlation:
   - Analyze the relationship between emotional patterns and loan terms (amount, interest rate).
   - Identify which emotional factors have the strongest influence on loan results.

4. Lending Operation Assessment:
   - Evaluate the effectiveness of the lending policy (interest rates and loan amount) in terms of the default
   - Measure growth and profitability of the lending operation.
   - Analyze disbushment, loan performance, and revenue trends over time.

5. Data Visualization and Dashboard:
   - Create a comprehensive dashboard with key metrics and insights from your analysis.
   - Include visualizations that effectively communicate complex emotional patterns and their relationship to loan data.

#### [Optional] Reasoning

- Suggest refinements to the emotional data collection process.
- Propose improvements to the loan approval algorithm.
- Recommend strategies for personalizing credit offers based on emotional patterns.
- Discuss the ethical implications of using emotional data for credit decisions.

#### [Optional] Machine Learning

- Create a model to predict loan terms based on emotional and contextual data.
- Evaluate the model's performance and identify the most important features.

### Technical Requirements

1. Use SQL for data extraction from the SQLite database.
2. Use Python for data preprocessing, analysis, and any machine learning tasks.
3. Use appropriate data visualization libraries for your exploratory data analysis and final dashboard.
4. Provide clear documentation for your code and analysis process.

### Evaluation Criteria

Your solution will be evaluated based on:

1. Depth and quality of data analysis and exploration
2. Clarity and actionability of insights and recommendations
3. Quality of data visualizations and dashboard
4. Presentation skills and ability to communicate complex findings
5. Code quality, organization, and documentation
6. Bonus points for completing the Optional and Reasoning sections:
   - Candidates who address the tasks in the Optional and Reasoning sections will receive additional points.
   - These sections demonstrate advanced analytical skills and a deeper understanding of the ethical implications of the ECS.

## Submission Guidelines

1. Provide your solution in a GitHub repository, including all code, notebooks, and SQL scripts.
2. Include a README.md with setup instructions and any assumptions you made.
3. Submit your dashboard (or presentation tool) along with explanations of the visualizations.
4. Prepare a presentation (30 minutes) summarizing your approach, key findings, and recommendations.

## DISCLAIMER

The Empathic Credit Limit System (ECS) described in this case study is entirely fictional. This concept was created solely for the purpose of this exercise and does not represent any real-world technology or system. The idea of using emotional data for credit decisions is purely hypothetical and is meant to stimulate creative thinking and analysis within the context of this technical case.

Good luck!
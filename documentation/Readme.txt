# FinOps Power BI Dashboard

## Project Overview

This project is a beginner-friendly FinOps dashboard built in Power BI using sample multi-cloud cost data.

The dashboard analyses cloud spend across AWS, Azure, and GCP, with a focus on cost visibility, tagging health, ownership, AI spend, and optimisation opportunities.

## Business Problem

Cloud costs are often difficult to manage when spend is spread across multiple cloud providers, departments, teams, and services.

FinOps teams need visibility into:

- Total cloud spend
- Spend by cloud provider
- Spend by department and team
- Untagged and partially tagged resources
- AI-related cloud spend
- Optimisation opportunities

This dashboard was created to show how Power BI can support FinOps decision-making.

## Tools Used

- Power BI Desktop
- Excel
- DAX
- Sample multi-cloud billing data

## Dashboard Pages

### 1. Executive Overview

This page shows:

- Total Cloud Spend
- Untagged Spend
- Untagged Spend %
- AI Spend %
- Cost by Cloud Provider
- Cost by Department
- Cost by Service Category
- Monthly Cloud Cost Trend

### 2. Tagging Health

This page focuses on governance and ownership.

It shows:

- Tagged vs Untagged Spend
- Untagged Spend by Team
- Partially tagged resources
- Resources requiring tagging action

### 3. Optimisation Opportunities

This page highlights areas where cloud cost can be reviewed.

It includes:

- Spend by optimisation recommendation
- Top expensive resources
- Service category cost by cloud provider

## Key FinOps Insights

From the sample dataset:

- AI workloads represent the largest share of cloud spend.
- Untagged and partially tagged resources create ownership and allocation challenges.
- Tagging quality is important for showback, chargeback, budgeting, and accountability.
- Optimisation should focus first on high-cost services and teams with poor tagging discipline.

## DAX Measures Used

```DAX
Total Spend = SUM('Cloud Cost'[Cost GBP])
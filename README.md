# HDFC Bank Service Request SLA Analyzer

##  Project Overview

The HDFC Bank Service Request SLA Analyzer is a data analytics project developed using Python, Pandas, and Google Colab. The main objective of this project is to understand how data analysis can help monitor customer service requests, identify potential delays, and organize requests according to their priority.

In the banking sector, customers raise service requests related to accounts, cards, loans, KYC verification, complaints, and digital banking. Managing these requests becomes challenging when information is stored across multiple datasets. An organized analytical process can help bring this information together and make it easier to evaluate service performance.

I developed this project to create a structured workflow for data loading, cleaning, validation, integration, SLA analysis, priority classification, and report generation.

The project uses simulated data for educational purposes. It demonstrates a data analytics approach to service request monitoring and should not be interpreted as an official representation of HDFC Bank's internal systems or actual operational performance.

##  Project Objectives

The main objectives of this project are:

- Load and organize multiple datasets using Python.
- Clean and validate data before performing analysis.
- Identify missing values, duplicate records, and potential data quality issues.
- Integrate customer, branch, ticket, update, complaint, and service request information.
- Calculate elapsed request time and compare it with predefined SLA limits.
- Identify potential SLA breaches according to the implemented business rules.
- Analyze request volumes and SLA performance at the branch level.
- Classify service requests into High, Medium, and Low priority categories.
- Generate recommended actions based on defined priority rules.
- Export analytical reports in CSV and Excel formats.
- Validate the final outputs to maintain consistency across the workflow.

##  Technologies Used

The project uses the following tools and technologies:

| Technology | Purpose |

| Python | Main programming language |
| Pandas | Data cleaning, transformation, merging, and aggregation |
| Google Colab | Writing and executing Python code |
| CSV | Reading datasets and exporting reports |
| Excel | Storing and reviewing summary reports |
| Data Validation | Checking data quality and consistency |
| Business Rules | Calculating SLA status and assigning priorities |


##  Key Learning Outcomes

Working on this project provided practical experience in several areas of data analytics.

I gained experience in using Pandas for data manipulation, integrating multiple datasets, implementing business rules, calculating SLA metrics, grouping records for summary analysis, and exporting reports.

I also learned why row-count reconciliation, identifier validation, and data-type checks are important in a multi-stage data workflow.

The project helped me understand how programming and data analysis can be applied to a business problem rather than being limited to isolated coding exercises.

## Project Workflow

The project follows a structured, step-by-step workflow to transform raw service request data into meaningful analytical reports.

### Step 1: Data Loading
Load the service request, customer, branch, support ticket, update, and complaint datasets into Python using Pandas.

### Step 2: Data Cleaning and Validation
Inspect the datasets, check missing values and duplicate records, validate data types, and identify data quality issues before performing further analysis.

### Step 3: SLA Calculation
Calculate the elapsed time for service requests and compare it with predefined Service Level Agreement (SLA) limits to identify potential SLA breaches.

### Step 4: Data Integration
Combine the cleaned datasets using relevant identifiers, such as request IDs, customer IDs, and branch IDs, to create a more complete view of each service request.

### Step 5: Branch-Level Analysis
Group service requests by branch and calculate metrics such as total requests, breached requests, and SLA breach rates.

### Step 6: Priority Classification
Apply predefined business rules using SLA breaches, severe open complaints, escalated tickets, and repeat requests to calculate priority scores and classify requests as High, Medium, or Low.

### Step 7: Recommended Actions
Generate suggested actions based on the implemented priority rules to help identify service requests that may require further attention.

### Step 8: Final Data Validation
Validate request counts, unique request IDs, priority classifications, summary totals, and breach-rate calculations to check the consistency of the results.

### Step 9: Report Generation
Prepare the detailed service request report, priority summary, and branch-level SLA summary.

### Step 10: Export and Review
Export the final reports into CSV and Excel formats for further analysis and review.

          ┌──────────────────────┐
          │   Input Datasets     │
          └──────────┬───────────┘
                     ↓
          ┌──────────────────────┐
          │ Data Cleaning &      │
          │ Validation           │
          └──────────┬───────────┘
                     ↓
          ┌──────────────────────┐
          │ SLA Calculation      │
          └──────────┬───────────┘
                     ↓
          ┌──────────────────────┐
          │ Data Integration     │
          └──────────┬───────────┘
                     ↓
          ┌──────────────────────┐
          │ Branch-Level Analysis│
          └──────────┬───────────┘
                     ↓
          ┌──────────────────────┐
          │ Priority Assignment  │
          └──────────┬───────────┘
                     ↓
          ┌──────────────────────┐
          │ Final Validation     │
          └──────────┬───────────┘
                     ↓
          ┌──────────────────────┐
          │ Reports & Exports    │
          └──────────────────────┘

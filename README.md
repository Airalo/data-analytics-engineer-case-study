# Senior Analytics Engineer — Take-Home Assignment

Thank you for your interest in the Senior Analytics Engineer role at Airalo. We were impressed with our conversation and would like to invite you to the next step: a take-home task designed to reflect the type of analytical challenges we work on. 

This should take approximately 4-5 hours to complete.

---

## Scenario

You are a Senior Analytics Engineer at Airalo, working closely with Growth, Product, and Marketing to understand customer purchasing behavior and revenue performance.

For instance, the business wants to understand: 

- Where to focus marketing spend (acquisition vs re-engagement)
- How often customers return to purchase additional eSIMs?
- How long it takes for customers to come back and buy again?

You are provided 2 datasets: 

- `users`
- `orders`

Your task is to transform this raw data into a clean, analytics-ready orders fact table that can be reliably used by downstream stakeholders for reporting and decision-making.

---

## Assignment

### 1. Data Setup

The data is provided as CSV files.  
You may load these files into a database of your choice (SQLite, PostgreSQL, BigQuery, or Snowflake).

---

### 2. Data Modelling

Using **dbt**, build an **orders fact table** supported by any upstream transformation models.  
Where applicable, ensure appropriate handling of duplicate records.

At a minimum, the final orders table should include:

- An indicator for new vs. returning customers
- The number of days between a customer’s first purchase and their most recent purchase

You may include additional derived fields or intermediate logic where necessary to support clarity, reusability, and analytical use cases.

**Note:** While dbt is preferred, we understand setup time can be a constraint. SQL-only submissions are acceptable if clearly structured and well documented.
---

### 3. Testing

Add **tests where appropriate** (e.g. uniqueness, not null, accepted values) to ensure data quality and reliability.

---

### 4. Written Response

Please write a short response covering the following:

**Logic Separation**  
How do you decide where to perform data cleaning versus where to implement more complex business logic?

---

## Evaluation Criteria

Submissions will be evaluated based on:

1. **Code Quality**  
   Is your SQL clean, readable, reusable, and easy to maintain?

2. **Data Modelling Best Practices**  
   We use dbt best practices as outlined here:  
   https://docs.getdbt.com/best-practices/how-we-style/0-how-we-style-our-dbt-projects

---

## Submission Instructions

Please submit:

- Your **dbt project** (or SQL files if dbt is not used)
- Any relevant **documentation or README**
- Your **written response**

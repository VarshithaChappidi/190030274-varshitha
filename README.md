# Bank Database Demo (SQL Server)

A small relational database exercise using Microsoft SQL Server / T-SQL. The schema models customers, banks/branches, and customer accounts, including primary keys and foreign-key relationships.

## Schema

- **`CUSTOMER`** — customer profile fields.
- **`BANK_INFO`** — bank and branch reference information.
- **`CUSTOMER_ACCOUNT`** — account details linked to a customer and a bank.

The script includes a join query to show customer, account, and bank information together.

## Run locally

1. Open SQL Server Management Studio (SSMS) or another SQL Server query editor connected to a development SQL Server instance.
2. Open `sqlquery`.
3. Execute the script from top to bottom. It creates the `DB_BANK` database if it does not already exist, creates the three tables, inserts sample rows, and runs example queries.

**Important:** This is a one-time setup script for a clean demo database. It does not drop or reset existing tables; rerunning it after the tables have been created will fail on the existing table names. Use a fresh demo database or intentionally reset your own demo tables before rerunning it.

## Data and security

- The included rows are fictional placeholders, not real customer records.
- Do not commit real names, phone numbers, addresses, email addresses, account numbers, or banking credentials.
- This is a learning example, not a production banking system. It does not implement authentication, authorization, encryption, transaction processing, or banking rules.

## Repository contents

- `sqlquery` — T-SQL schema, fictional seed data, and example queries.

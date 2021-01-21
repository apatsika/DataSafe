# Discover and Mask Sensitive Data

## Introduction

This lab shows you how to discover and mask sensitive data in your Autonomous Database by using the Data Discovery and Data Masking features in Oracle Data Safe.

Estimated Lab Time: **30 minutes**

## Objectives

In this lab, you'll:

- View sensitive data in your database
- Discover sensitive data in your database by using the Data Discovery feature
- Mask sensitive data in your database by using the Data Masking feature
- Create a PDF of the Data Masking report
- Validate the masked data in your database

## Prerequisites

To complete this lab, you need to have the following:

- An Oracle Cloud account
- Access to an Oracle Database as the `SYS` user, sample data for Oracle Data Safe loaded into the database, and the Discovery and Masking features enabled on your database
- Access to an Oracle Data Safe service
- Privileges to use the Discovery and Masking features on your database

### STEP 1: View sensitive data in your database

In this step, you use SQL Developer to query sensitive data in your database.

```
alter session set container=<YOUR PDB NAME>
```

Next, run the following statem statement

```
select * from HCM1.employees;
```

Review the query results.

- Data such as employee_id, first_name, last_name, email, phone_number, and hire_date, are considered sensitive data and should be masked if shared for non-production use, such as development and analytics.
- Keep this tab open so that you can return to it later. In step 4, you compare the original query results with the masked data.

![Select all employees](images/select-all.png)

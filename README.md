# Customer Data Cleaning with Python and Pandas

## Overview

This repository documents a customer-data preprocessing project using Python and Pandas. The goal was to improve the consistency and usability of a customer call list originally stored in Excel.

## Objectives

- Remove duplicate rows.
- Remove an unwanted column.
- Clean inconsistent surname formatting.
- Handle missing and placeholder values.
- Standardize phone-number formatting.
- Split address information into separate columns.
- Normalize customer-status categories.
- Apply documented record-filtering rules.
- Export the processed dataset to Excel.

## Tools and Technologies

- Python
- Pandas
- Jupyter Notebook
- Microsoft Excel

## Workflow

1. I Load the Excel dataset into a Pandas DataFrame.
2. I Inspect the source records and fields.
3. I Remove duplicate rows.
4. I Drop the unwanted column.
5. I Clean text values in the surname field.
6. I Handle missing and placeholder values.
7. I Standardize phone numbers.
8. I Split address components.
9. I Normalize paying-customer and do-not-contact values.
10. I Apply record-filtering rules.
11. I Reset the DataFrame index.
12.  I Export the resulting dataset to Excel.



## Key Learning Outcomes

- Practical use of Pandas for data manipulation.
- Applying string methods and regular expressions.
- Handling missing values and placeholders.
- Restructuring combined fields.
- Standardizing categorical data.
- Exporting cleaned data.
- Recognizing the importance of validation and data provenance.

## Quality Improvements to Complete

Before treating the output as production-ready, validate phone-number lengths, review missing-value treatment, verify address parsing, check the effect of record filters, and compare before-and-after row counts.

## Conclusion

This project demonstrates a practical data-cleaning workflow and highlights the importance of data quality in the analytics lifecycle.

**Author:** Adegbola Oluwakemi Esther

**Primary technologies:** Python, Pandas, Jupyter Notebook, Excel

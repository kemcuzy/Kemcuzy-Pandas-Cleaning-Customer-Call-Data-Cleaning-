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
3. I Remove duplicate rows. I used drop_duplicates() to remove exact duplicate records. This helped reduce redundant rows, although identifying duplicate customers across different records would require additional checks.
4. I Drop the unwanted column.
5. I Clean text values in the surname field, I applied Pandas string methods to remove unwanted characters from the surname field. This highlighted how string manipulation can help standardize text without manually editing each record.
6. I Handle missing and placeholder values, by exploring fillna() and replaced missing or placeholder values with blanks in the working dataset. This step also highlighted an important data-quality lesson: missing customer information should not be replaced with invented details unless there is a verified basis for doing so.
7. I Standardize phone numbers, I used regular expressions and string slicing to remove unwanted separators and attempt a consistent phone-number format. This demonstrated the usefulness of programmatic transformations while showing why length checks and missing-value handling are necessary.
8. I Split address components, by splitting the combined address field into separate components. This made the information more structured, although the resulting fields still require validation against the original address format.
9. I Normalize paying-customer and do-not-contact values by converting Yes/No values in the paying-customer and do-not-contact fields to Y/N. Standardizing categories makes subsequent filtering and grouping more dependable.
10. I Apply record-filtering rules, by removing records according to the notebook's do-not-contact and blank-phone-number conditions. 
11. I Reset the DataFrame index by making use of df = df.reset_index(drop=True)
12.  I Export the resulting dataset to Excel.



## Key Learning Outcomes

- Practical use of Pandas for data manipulation.
- Applying string methods and regular expressions.
- Handling missing values and placeholders.
- Restructuring combined fields.
- Standardizing categorical data.
- Exporting cleaned data.
- Recognizing the importance of validation and data provenance.




##Post-Analysis Insights

This project strengthened my understanding of three important principles.

First, cleaning is a structured process that requires field-level decisions. Second, consistent formatting does not automatically mean that a value is valid. hird, Tmissing values and contact preferences must be handled in ways that preserve the meaning of the original information.


## Conclusion

This project demonstrates a practical data-cleaning workflow and highlights the importance of data quality in the analytics lifecycle.

**Author:** Adegbola Oluwakemi Esther

**Primary technologies:** Python, Pandas, Jupyter Notebook, Excel

# README – Excel Assignment 2: Data Cleaning and Transformation

## Overview
This document summarizes the data cleaning, transformation, and formatting activities performed on the product dataset.

## 1. Handling Missing Values

### Missing Values in the Price Column
| Product Brand | Original Price | Clean Price |
|--------------|---------------|------------|
| Headphones Sony | Blank | $250.00 |
| Sunglasses Ray-Ban | Blank | $150.00 |

### Approach Used
- Retained the original **Price ($)** column for reference.
- Created a **Price Clean** column to store corrected values.
- Missing prices were filled using reference prices from similar products or category-based estimates.
- Records without reliable prices should be reviewed manually.

### Missing Values in the Category Column
| Product Brand | Category Clean |
|--------------|---------------|
| Backpack North Face | Outdoor |
| Sneakers Adidas | Fashion |
| Coffee Maker Nespresso | Kitchen |
| Fitness Tracker Xiaomi | Electronics |

Formula used:
```excel
=IF(ISBLANK([@[Category Old]]),VLOOKUP([@[Product Name - Copy]],Categories,2,FALSE),[@[Category Old]])
```

## 2. Correcting Inconsistent Data

### Product Name Standardization
- Converted all product names to Proper Case.
- Standardized capitalization across the dataset.

Examples:
- laptop → Laptop
- smartphone → Smartphone
- headphones → Headphones

### Category Typo Corrected
- Electroni → Electronics

## 3. Removing Duplicates

- Duplicate records were identified based on the entire row.
- Duplicates were removed using Power Query Editor.
- The first occurrence of each record was retained.

## 4. Splitting and Merging Data

### Split Product ID
The Product ID field was split into:
- Manufacturing Date
- Country Code

Example:
- 28-01-2026 | US

### Merge Product Name and Brand Name
A new column **Product Brand** was created.

Examples:
- Laptop + Dell → Laptop Dell
- Smartphone + Samsung → Smartphone Samsung

## 5. Number Formatting

### Price Formatting
Applied Currency format:
- $1,000.00
- $80.00
- $130.00

### Manufacturing Date Formatting
Format used:
- DD-MM-YYYY

Example:
- 28-01-2026

## 6. Conditional Formatting

### Price Column
Applied:
- Data Bars
- Color Scales

### Category Column
Custom rule:
- Cell Value = "Electronics"

Formatting:
- Green fill color
- Bold font

## Deliverables Completed

- Missing price values handled
- Missing category values populated
- Product names standardized
- Category typo corrected
- Duplicate records removed
- Product ID split into Manufacturing Date and Country Code
- Product Name and Brand Name merged into Product Brand
- Price formatted as Currency
- Manufacturing Date formatted as DD-MM-YYYY
- Conditional formatting applied
- Final cleaned dataset prepared successfully

## Conclusion

The dataset has been cleaned, standardized, transformed, and formatted according to the assignment requirements.

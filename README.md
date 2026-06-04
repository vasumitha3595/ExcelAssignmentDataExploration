# Excel Formula Assignment Documentation

## Dataset Overview

The dataset contains product information including Product ID, Product Name, Brand Name, Price, Quantity, Category, Date, Country Code, and Month. Various Excel formulas were used to analyze and manipulate the data.

---

# 1. SUM Function

### Formula

```excel
=SUM(Table[Price ($)])
```

### Purpose

Calculates the total of all values in the Price column.

### Steps

1. Select the result cell.
2. Enter the formula.
3. Press Enter.
4. Excel adds all prices together.

### Result

**10100**

---

# 2. COUNTA Function

### Formula

```excel
=COUNTA(Table[Product Name])
```

### Purpose

Counts all non-empty cells in the Product Name column.

### Steps

1. Select an empty cell.
2. Type the formula.
3. Press Enter.
4. Excel counts all product names.

### Result

**34**

---

# 3. AVERAGE Function

### Formula

```excel
=AVERAGE(Table[Price ($)])
```

### Purpose

Calculates the average price of all products.

### Steps

1. Select the output cell.
2. Enter the formula.
3. Press Enter.
4. Excel calculates the mean value.

### Result

**297.06**

---

# 4. MIN Function

### Formula

```excel
=MIN(Table[Price ($)])
```

### Purpose

Finds the lowest price in the dataset.

### Steps

1. Select an empty cell.
2. Enter the formula.
3. Press Enter.
4. Excel returns the smallest value.

### Result

**30**

---

# 5. MAX Function

### Formula

```excel
=MAX(Table[Price ($)])
```

### Purpose

Finds the highest price in the dataset.

### Steps

1. Select a result cell.
2. Enter the formula.
3. Press Enter.
4. Excel returns the largest value.

### Result

**1000**

---

# 6. IF Function

### Formula

```excel
=IF([@Price ($)]>=500,"high price","standard price")
```

### Purpose

Categorizes products based on price.

### Logic

* If Price ≥ 500 → High Price
* Otherwise → Standard Price

### Steps

1. Create a new column named Price Range.
2. Enter the formula in the first row.
3. Press Enter.
4. Fill down the column.

### Example Output

| Price | Result         |
| ----- | -------------- |
| 1000  | high price     |
| 130   | standard price |
| 500   | high price     |

---

# 7. SUMIF Function

### Formula

```excel
=SUMIF(Table[Category],M8,Table[Price ($)])
```

### Purpose

Adds prices for products belonging to a specific category.

### Steps

1. Enter the category name in a reference cell (e.g., Electronics).
2. Use the SUMIF formula.
3. Press Enter.
4. Excel sums prices matching the category.

### Example Result

**8050** (Electronics Category)

---

# 8. COUNTIF Function

### Formula

```excel
=COUNTIF(Table[Price ($)],"<1")
```

### Purpose

Counts cells meeting a specified condition.

### Steps

1. Select a result cell.
2. Enter the formula.
3. Press Enter.
4. Excel counts records matching the criteria.

### Result

**11**

---

# 9. LEFT Function

### Formula

```excel
=LEFT([@[Product ID]],2)
```

### Purpose

Extracts the first two characters from Product ID.

### Steps

1. Create a new column.
2. Enter the formula.
3. Press Enter.
4. Fill down if necessary.

### Example

| Product ID | Result |
| ---------- | ------ |
| 28-JAN-US  | 28     |
| 15-FEB-US  | 15     |

---

# 10. RIGHT Function

### Formula

```excel
=RIGHT([@[Product ID]],2)
```

### Purpose

Extracts the last two characters from Product ID.

### Steps

1. Select a new column.
2. Enter the formula.
3. Press Enter.
4. Copy down.

### Example

| Product ID | Result |
| ---------- | ------ |
| 28-JAN-US  | US     |
| 07-JUN-UK  | UK     |

---

# 11. MID Function

### Formula

```excel
=MID([@[Product ID]],4,3)
```

### Purpose

Extracts characters from the middle of Product ID.

### Steps

1. Select a result cell.
2. Enter the formula.
3. Press Enter.
4. Fill down.

### Example

| Product ID | Result |
| ---------- | ------ |
| 28-JAN-US  | JAN    |
| 03-MAR-US  | MAR    |

---

# Summary Table

| Formula | Purpose                             |
| ------- | ----------------------------------- |
| SUM     | Adds all values                     |
| COUNTA  | Counts non-empty cells              |
| AVERAGE | Finds average value                 |
| MIN     | Finds smallest value                |
| MAX     | Finds largest value                 |
| IF      | Applies conditional logic           |
| SUMIF   | Sums values based on criteria       |
| COUNTIF | Counts values based on criteria     |
| LEFT    | Extracts characters from left side  |
| RIGHT   | Extracts characters from right side |
| MID     | Extracts characters from the middle |

## Conclusion

This assignment demonstrates the use of common Excel functions for data analysis, conditional calculations, aggregation, and text manipulation. Structured table references were used to make formulas dynamic and easier to manage.

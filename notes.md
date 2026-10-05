# Copilot DAX Development Notes

## 1. Total Sales

### Copilot suggestion
Copilot suggested using the SUM function to add the sales amount values from the Fact_Sales table.

### Final version
The final measure uses `SUM(Fact_Sales[sales_amount])` to calculate total sales.

### Changes
I checked that `sales_amount` was the correct field in the Fact_Sales table. No major correction was needed.

---

## 2. MoM Growth %

### Copilot suggestion
Copilot suggested using CALCULATE and DATEADD to compare the current month's sales with the previous month's sales.

### Final version
The final measure calculates the percentage change between current-month and previous-month sales.

### Changes
I changed the date reference to `Dim_Date[date]` so that the calculation matched my date table and worked correctly with the report's date context.

---

## 3. Running Total Sales

### Copilot suggestion
Copilot suggested using CALCULATE with FILTER to calculate cumulative sales over time.

### Final version
The final measure uses ALLSELECTED together with the maximum selected date to calculate running total sales.

### Changes
I adjusted the date context so that the running total responds to the filters selected in the report.

---

## 4. City Sales Rank

### Copilot suggestion
Copilot suggested using the RANKX function with the city dimension to rank cities by their sales.

### Final version
The final measure ranks cities based on Total Sales.

### Changes
I used descending order with DENSE ranking so that the city with the highest sales receives rank 1.

---

## 5. Average Transaction Value

### Copilot suggestion
Copilot suggested calculating the average transaction value by dividing total sales by the number of transactions.

### Final version
The final measure uses DIVIDE to calculate the average transaction value safely.

### Changes
I checked the calculation against the Fact_Sales transaction data and verified the result in the Power BI dashboard.

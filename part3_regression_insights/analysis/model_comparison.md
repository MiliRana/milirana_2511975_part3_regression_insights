# Model Comparison

## Model 1: Simple Regression (Marketing Spend)

### Variables

* Dependent Variable: monthly_sales
* Independent Variable: marketing_spend

### Results

* R-squared: 0.167
* Significant Variable:

  * marketing_spend (p-value < 0.001)

### Business Usefulness

Marketing spend has a positive relationship with sales. Higher marketing expenditure is associated with higher monthly sales.

### Limitations

The model explains only 16.7% of sales variation, meaning many important factors are not included.

---

## Model 2: Simple Regression (Footfall)

### Variables

* Dependent Variable: monthly_sales
* Independent Variable: footfall

### Results

* R-squared: 0.736
* Significant Variable:

  * footfall (p-value < 0.001)

### Business Usefulness

Footfall is strongly associated with sales. Stores with higher customer traffic generally generate higher sales.

### Limitations

The model ignores other factors such as marketing, inventory availability, and store type.

---

## Model 3: Multiple Regression (Final Model)

### Variables

Dependent Variable:

* monthly_sales

Independent Variables:

* marketing_spend
* footfall
* inventory_availability_pct
* Store_Mall (dummy variable)

### Results

* R-squared: 0.809
* Significant Variables:

  * marketing_spend (p < 0.001)
  * footfall (p < 0.001)
  * inventory_availability_pct (p < 0.001)
  * Store_Mall (p = 0.009)

### Business Usefulness

This model provides the strongest explanation of monthly sales and captures multiple operational factors simultaneously.

### Limitations

The model does not capture all influences on sales, such as local competition, customer preferences, economic conditions, or seasonality.

---

## Overall Comparison

| Model               | R-Squared |
| ------------------- | --------- |
| Marketing Spend     | 0.167     |
| Footfall            | 0.736     |
| Multiple Regression | 0.809     |

The multiple regression model is selected as the final model because it explains the highest percentage of variation in monthly sales while using several significant business drivers.

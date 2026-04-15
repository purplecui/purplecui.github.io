

# Consumer Theory: Analytical and Computational Framework

---

## 1. Conceptual Foundation

Consumer theory is built on the premise that individuals seek to maximize utility subject to a budget constraint. This optimization problem reflects the fundamental economic condition of scarcity, where limited income must be allocated across competing uses.

The theory assumes that consumers have well-defined preferences that are complete and transitive, allowing them to rank all possible bundles of goods.

---

## 2. Utility Maximization Problem

The formal problem can be expressed as:

Maximize U(X, Y)  
Subject to: PxX + PyY = Income

This leads to the condition:

MUx / MUy = Px / Py

This condition equates the marginal rate of substitution with the market price ratio, representing a balance between subjective valuation and objective constraints.

---

## 3. Computational Illustration in R

### Example: Cobb-Douglas Utility Function

U(X, Y) = X^0.5 * Y^0.5

```r
# Define parameters
income <- 100
Px <- 2
Py <- 1

# Optimal consumption for Cobb-Douglas
X_opt <- (0.5 * income) / Px
Y_opt <- (0.5 * income) / Py

X_opt
Y_opt

```


## 4. Interpretation of Results

The solution indicates that the consumer allocates a fixed proportion of income to each good, reflecting the structure of the utility function. This proportional allocation is a distinctive feature of Cobb-Douglas preferences.

---

## 5. Sensitivity Analysis in R

Consumer theory provides a structured way to understand decision-making, but its real strength lies in its adaptability. When implemented computationally, it allows for simulation of diverse economic environments, bridging the gap between theoretical abstraction and empirical reality.

```R
# Vary income levels  
income_values <- seq(50, 200, by = 10)  
  
X_values <- (0.5 * income_values) / Px  
Y_values <- (0.5 * income_values) / Py  
  
data.frame(income_values, X_values, Y_values)

```
---

## 6. Interpretation Questions

1. How would the optimal consumption bundle change if preferences were not symmetric (e.g., U = X^0.7 * Y^0.3)?
2. What happens to consumption choices when the price of one good increases significantly?
3. How does the structure of the utility function influence demand behavior?
4. In what ways does real-world consumer behavior deviate from the assumptions of this model?

---

## 7. Analytical Insight

Consumer theory provides a structured way to understand decision-making, but its real strength lies in its adaptability. When implemented computationally, it allows for simulation of diverse economic environments, bridging the gap between theoretical abstraction and empirical reality.
# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:**

This is a **regression** problem because species richness is a **numerical** outcome. We are interested in **inference** to understand which predictors affect species richness. Here, **n = 200** and **p = 4** because **predictors** are reserve size, years since establishment, enforcement budget, and proximity to human settlements.

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and **eight** other variables.

> **Your Answer:**

This is a **classification** problem because the outcome is **categorical** (successful or unsuccessful). We are interested in **prediction** because the goal is to predict whether a proposed habitat corridor will succeed or fail. We have  **n = 30** and **p = 11* because the **predictors** are corridor width, length, surrounding land use type, and eight other variables.

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric conditions.

> **Your Answer:**

This is a **regression** problem because ozone concentration is a  **numerical** outcome. We are interested in **prediction** because the goal is to predict ozone levels. Since the data are weekly for one year, **n = 52**. Based on the variable listed, **p = 4** if the **predictors** are sea surface temperature, wind speed, solar radiation, and atmospheric conditions. The ozone concentration is not counted in **p** because it is the response variable.

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:**

A **very flexible** method can fit more complicated relationships, so it may give better predictions when the true pattern is not simple. The disadvantage of such a method may be overfitting, which can fit noise in the training data rather than the true pattern, and it may also be hard to interpret. 

A flexible model is preferred when we have lots of data and mainly care about making accurate predictions, while a less flexible model is better when we have less data or when we are interested in inference and understanding how the predictors affect the response, since simpler models are easier to interpret.

---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:** 

A **parametric** approach assumes a specific form for the relationship between **predictors** and the **response** (ex. linear relationship). A **non-parametric** approach does not assume a fixed form and is more flexible. 

The disadvantage of the parametric approach is that it can perform poorly if the assumed form is incorrect, as it is too restrictive. Non-parametric methods can capture more complex patterns, but they have the disadvantage of often requiring more data, being harder to interpret, and being more prone to overfitting.


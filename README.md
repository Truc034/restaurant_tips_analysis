# 🍽️ Restaurant Tips Analysis

## Project description
This project aims to use the restaurant tips dataset to practice creating composition plots and visualizations. We will examine the relationship between different variables and the tips given.

![image](https://github.com/user-attachments/assets/5cbc2051-9678-4cd6-83a2-8c1ab99fd2b2)

## Data description

### Data source
This project aims to use the restaurant tips dataset to practice creating composition plots and visualizations. We will examine the relationship between different variables and the tips given.

The dataset consists of information from 244 restaurant bills, collected in the US in 1987.

It includes details about the tips given to restaurant staff, such as the total bill, tip amount, gender of the person paying, smoking status, day of the week, time of day, and party size.
The dataset is publicly available and sourced from the GitHub repository of RusAbk’s SCA datasets collection.
**Link**: https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv

### Dataset description
The dataset includes transactional data from a restaurant. Each row represents a single customer's bill, containing the following attributes:
+ **total_bill**: Total bill in USD
+ **tip**: Tip amount in USD
+ **sex**: Gender of the customer
+ **smoker**: Whether the customer is a smoker or non-smoker
+ **day**: Day of the week
+ **time**: Lunch or Dinner
+ **size**: Number of people at the table

### Data access
#### 📥 Data import
First, let's import the needed libraries: Pandas & Matplotlib.
`
import pandas as pd
import matplotlib.pyplot as plt
`

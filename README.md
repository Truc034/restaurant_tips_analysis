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

### 📥 Data access
First, let's import the needed libraries: Pandas & Matplotlib.
``` python
import pandas as pd
import matplotlib.pyplot as plt
```

The dataset is not stored locally in the repository, but it can be directly accessed via the raw GitHub URL provided above. In the notebook, it's read using:
``` python
df = pd.read_csv('https://raw.githubusercontent.com/RusAbk/sca_datasets/main/tips.csv')
```

### 🔍 Data exploration
Let's take a look at the first 5 rows to be sure, that data is loaded properly:
``` python
df.head(5)
```
![image](https://github.com/user-attachments/assets/9acc5744-3c4a-4df1-b98e-626acf40a94a)

Show the columns of the dataframe and their types:
``` python
df.info()
```

![image](https://github.com/user-attachments/assets/11a3052e-0601-4753-b15e-ccbdaf7baf40)

As you can see each observation represents a customer who left a tip at a restaurant.
We can see information about:
+ **total_bill**: Total bill in USD
+ **tip**: Tip amount in USD
+ **sex**: Gender of the customer
+ **smoker**: Whether the customer is a smoker or non-smoker
+ **day**: Day of the week
+ **time**: Lunch or Dinner
+ **size**: Number of people at the table

### Main goals
* Understand the overall distribution of tip values as well as within specific subgroups
* Analyze tipping behaviors in relation to gender, meal times (including days of the week or lunch vs dinner), and smoking status
* Detect outliers or noteworthy patterns (e.g., large tip values, tight ranges)
* Extract actionable insights via statistical analysis and visual storytelling

### Results

#### 🔍 Summary of exploration
The analysis investigates tipping patterns across various customer segments:
* Smoking Status: Smokers show a slight inclination to tip more than non-smokers, though the overall difference is not significant. 
* Gender: Male customers tend to tip a bit more and display a wider range in tipping behavior, including more frequent high-value tips.
* Day of Week: Weekend usually leave larger tips than weekday, possibly reflecting more relaxed or celebratory dining occasions.
* Meal Time: Tips given during dinner are generally higher and more varied compared to lunch, implying a difference in dining context or spending habits.

#### 📊 Visual Evidence
Each of these insights is visualized in grouped histograms showing tip distributions by:
+ Smoking Status
+ Gender
+ Day Type
+ Meal Time

📓 For detailed breakdowns and plots, view the [full notebook here].(https://github.com/Truc034/restaurant_tips_analysis/blob/main/Restaurant_tips_analysis.ipynb)

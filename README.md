# Titanic_Visualiazation

Titanic Survival Analysis
Dataset Description
This project analyzes the Titanic dataset to explore the factors that influenced passenger survival during the disaster. The dataset contains various features for each passenger, including:

survived: Survival status (0 = No, 1 = Yes)
pclass: Passenger class (1st, 2nd, 3rd)
sex: Sex of the passenger
age: Age in years
sibsp: Number of siblings/spouses aboard
parch: Number of parents/children aboard
fare: The fare paid
embarked: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
class: Passenger class (categorical)
who: Man, woman, or child
adult_male: Whether the passenger is an adult male
deck: Deck the passenger was on
embark_town: Port of embarkation (full name)
alive: Survival status (yes or no)
alone: Whether the passenger was alone
Visualizations
Below are screenshots of the visualizations generated to explore the data.

Distribution of Age
<img width="1074" height="626" alt="image" src="https://github.com/user-attachments/assets/a16d752b-f742-40a6-a3a0-7833eb0b66d4" />


Number of Survivors and Non-Survivors

<img width="1085" height="620" alt="image" src="https://github.com/user-attachments/assets/4568ae68-c8ca-45d5-bfbb-4b32c92591aa" />

Survival Rate by Passenger Class
<img width="1190" height="629" alt="image" src="https://github.com/user-attachments/assets/400aa656-45c0-45f1-bf00-7ec19d611794" />


Age Distribution by Survival
<img width="1081" height="648" alt="image" src="https://github.com/user-attachments/assets/195e8951-dcfd-41a7-9ba0-df132356345c" />


Fare Distribution by Survival
<img width="990" height="590" alt="Screenshot 2025-09-16 223222" src="https://github.com/user-attachments/assets/ea08ea61-035b-4229-aaee-17ee463cc5d5" />


Correlation Matrix of Numerical Features
<img width="1067" height="873" alt="Screenshot 2025-09-16 223446" src="https://github.com/user-attachments/assets/02afef0b-c61c-4bb2-a766-5870a219cb52" />

Insights from the visualizations:
------------------------------

1. Histogram of Age:
   - The age distribution is somewhat right-skewed, with a peak around the late 20s to early 30s.
   - There's a noticeable peak for very young passengers (around age 0-5).
   - The distribution is spread across a wide range, indicating diverse age groups on board.

2. Countplot of Survival:
   - There were significantly more non-survivors than survivors.
   - This indicates the majority of passengers on the Titanic did not survive the disaster.

3. Bar plot of Survival Rate by Passenger Class:
   - There is a clear trend: higher passenger classes (1st class) had a significantly higher survival rate compared to lower classes (2nd and 3rd class).
   - 3rd class had the lowest survival rate.
   - This suggests that passenger class was a strong predictor of survival.

4. Box plot of Age by Survival:
   - The median age for both survivors and non-survivors appears to be similar, around the late 20s or early 30s.
   - However, the age distribution for non-survivors seems slightly wider, with some older individuals among the non-survivors.
   - There are outliers in both groups, particularly among survivors, with some older individuals surviving.

5. Violin plot of Fare by Survival:
   - Passengers who paid higher fares (indicating higher class) had a much higher chance of survival.
   - The distribution of fares for survivors is heavily skewed towards higher values, while for non-survivors, it's concentrated at lower values.
   - This reinforces the observation from the passenger class plot that wealth or class was associated with survival.

6. Heatmap of the Correlation Matrix:
   - 'fare' and 'pclass' show a strong negative correlation (-0.55), which is expected as higher classes pay higher fares.
   - 'survived' has a moderate positive correlation with 'fare' (0.26) and a moderate negative correlation with 'pclass' (-0.34), supporting the findings that higher class and fare are associated with higher survival rates.
   - 'sibsp' and 'parch' have a moderate positive correlation (0.41), suggesting that people traveling with siblings/spouses are likely to also be traveling with parents/children.
   - 'age' has weak correlations with most other numerical features.

Comprehensive Analysis:
------------------------------
Based on the visualizations, the following key insights are derived:
1. Survival on the Titanic was not random. There was a significant disparity in survival rates.
2. Passenger class and the fare paid were strongly correlated with survival. Passengers in higher classes who paid more had a much greater probability of surviving.
3. While age distribution was broadly similar between survivors and non-survivors, the extreme ends of the age spectrum (very young and very old) seem to have different survival patterns, though this is less pronounced than the effect of class/fare.
4. The majority of passengers did not survive.
5. The correlation matrix confirms the relationships observed in individual plots, particularly the strong negative correlation between fare and passenger class and the positive correlation between fare/survival and negative correlation between pclass/survival.

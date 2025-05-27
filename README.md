# PSID-Education-Income-Study
A Statistical Analysis Using PSID Data

This project presents a comprehensive analysis of how educational attainment influences household income in the United States. Leveraging the 1993 cross-sectional dataset from the Panel Study of Income Dynamics (PSID), we apply rigorous statistical modeling to quantify the economic returns of education while controlling for relevant demographic and work-related factors.

🧩 Research Objective
Research Question:
How does educational attainment impact household income, when controlling for other socioeconomic variables such as age, hours worked, marital status, and number of children?

This analysis aims to provide empirical evidence to support policy and personal decision-making regarding the economic value of education.

📁 Dataset Overview
Source: Panel Study of Income Dynamics (PSID)

Year Used: 1993 (cross-sectional sample)

Sample Size: 3,454 individuals

Key Variables:

education: Years of formal schooling

log_income: Log-transformed total household income

age, age_squared: Age and its polynomial term

hours_worked: Total annual work hours

children: Number of dependent children

marital_status: One-hot encoded categorical variable


📊 Methodology
1. Data Preprocessing
Removed missing or invalid values

Applied log(1 + income) transformation

Created age_squared and hourly wage features

Encoded marital status into dummy variables

2. Exploratory Data Analysis (EDA)
Visualized distributions and outliers using histograms and boxplots

Correlation analysis to detect multicollinearity

Scatter plots to evaluate trends and non-linearities

3. Regression Modeling
A multiple linear regression model (OLS) was fit using:

𝑙
𝑜
𝑔
𝑖
𝑛
𝑐
𝑜
𝑚
𝑒
=
𝛽
0
+
𝛽
1
(
𝑒
𝑑
𝑢
𝑐
𝑎
𝑡
𝑖
𝑜
𝑛
)
+
𝛽
2
(
𝑎
𝑔
𝑒
)
+
𝛽
3
(
𝑎
𝑔
𝑒
2
)
+
𝛽
4
(
ℎ
𝑜
𝑢
𝑟
𝑠
𝑤
𝑜
𝑟
𝑘
𝑒
𝑑
)
+
𝛽
5
(
𝑐
ℎ
𝑖
𝑙
𝑑
𝑟
𝑒
𝑛
)
+
𝛽
6
−
9
(
𝑚
𝑎
𝑟
𝑖
𝑡
𝑎
𝑙
𝑠
𝑡
𝑎
𝑡
𝑢
𝑠
)
+
𝜀
log 
i
​
 ncome=β 
0
​
 +β 
1
​
 (education)+β 
2
​
 (age)+β 
3
​
 (age 
2
 )+β 
4
​
 (hours 
w
​
 orked)+β 
5
​
 (children)+β 
6
​
 − 
9
​
 (marital 
s
​
 tatus)+ε
R² Score: 0.465

Key Coefficient: Education (0.108) – each additional year of education is associated with a 10.8% increase in income, holding other variables constant.

🔍 Key Insights
Education is the most significant and stable predictor of income.

Children and marital status also impact household income.

Hours worked show a strong linear relationship with income.

Age does not show a statistically significant effect once squared terms are included.


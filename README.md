# Welcome to the Portfolio of Raiss Mounir 🎓📊

hamza ouad

### Table of contents
- [About Me ](#about-me)
- [Skills and Expertise ](#skills-and-expertise)
- [What You'll Find Here ](#what-youll-find-here)
- [Projects Showcase ](#projects-showcase)
- [Project N°1 (sales analysis project)(Python)](#project-n1-sales-analysis-project)
- [Project N°2 (HR Attrition Analysis)(Python & Power BI) ](#project-n2-hr-attrition-analysis)
- [Project N°3 — Work in Progress](#project-n3-in-progress)


### About Me 

#### Hello! I'm Raiss Mounir, a dedicated Data Analyst and Econometrician with a solid background in economics, data analytics, and applied research. I am passionate about transforming complex datasets into meaningful insights that empower informed decision-making. Holding a Master’s degree in Applied Econometrics, I excel at leveraging statistical tools and programming languages such as Python, R, SQL and Stata to uncover patterns, design predictive models, and solve real-world problems. Beyond technical expertise, I bring a collaborative mindset, meticulous attention to detail, and a strong commitment to delivering impactful results in every project.

###  Skills and Expertise 
- Data Cleaning, Analysis, and Visualization

- Econometric Modeling (Panel Data, Time Series, Cross Section)
 
- Statistical Programming (Python, R, SQL, Stata)

- Predictive Analytics 

- Dashboard Development (Power BI, excel)

###  What You'll Find Here 
This portfolio showcases my projects, skills, and achievements, including:

📊 Interactive dashboards for visualizing key trends and metrics.

📈 Advanced econometric models for real-world problem-solving.

### Projects Showcase 

Here are some of the key projects I’ve worked on, highlighting my skills in data analysis, econometrics, and visualization. Each project tackles a unique challenge and demonstrates my ability to transform data into actionable insights:

### Project N°1 Sales analysis project

#### Table of contents
- [Title](#project-title)
- [Project Description](#project-description)
- [Project Objectives](#project-objectives)
- [Tools Used](#tools)
- [Python Data Cleaning & Visualization](#data-cleaning-and-visualization-python)
- [Step 1: Importing Necessary Packages ](#step-1-setup-and-package-imports)
- [Step 2 Importing the Dataset ](#step-2-dataset-import)
- [Step 3: Verifying the Dataset ](#step-3-inspecting-the-dataset)
- [Step 4: Analyzing the Data — Answering the Business Questions ](#step-4-analyzing-the-data-answering-the-business-questions)


#### Project Title  
Sales analysis project

#### Project Description

This project is a data analysis case study aimed at understanding key trends and insights from a sales dataset of a company selling smartphones and gadgets. By analyzing the data, we can uncover important patterns regarding sales performance, product popularity, and customer behavior. The analysis helps answer several business-related questions and provides actionable insights for improving sales strategies.

### Project Objectives:
Identify the Month with the Highest Revenue: Determine which month generated the highest sales, providing insights into seasonality or trends.
Analyze the City with the Most Orders: Identify which city recorded the highest number of sales, helping the company to understand where its products are most popular.
Determine the Optimal Time for Advertising Campaigns: Analyze the data to recommend the best time for advertising campaigns to maximize sales.
Find the Best-Selling Product: Identify the product that sold the most and explore the factors contributing to its success.


#### Tools 

- Python for data cleaning and visualisation


###  Data Cleaning and Visualization Python

#### Step 1 Setup and Package Imports

The first step in any data analysis project is to import the necessary packages or libraries. These libraries provide the functions and tools needed to manipulate the data, perform computations, and create visualizations. Below is the code I used to import the required packages for this project:

![image](https://github.com/user-attachments/assets/ff0f27ac-525c-4cb7-90a6-886591190cab)

#### Step 2 Dataset Import
 
The next step in our analysis is importing the dataset into our Python environment. In this case, we have multiple files, each containing data for a specific month. These files need to be combined into a single, comprehensive dataset to analyze the entire year's worth of sales data.
We used the pandas library, which is an excellent tool for loading and manipulating data in Python. 
We first collect the names of all the CSV files in the directory where the monthly sales data is stored.

![image](https://github.com/user-attachments/assets/787b9983-8294-4252-982f-8fceacff533d)

Since we have data in multiple files, we need to combine them into one large dataset. To do this, we create an empty DataFrame (all_data) and loop through each file, reading it with pd.read_csv() and appending it to all_data using pd.concat().

![image](https://github.com/user-attachments/assets/47bce912-1bd4-439c-ad42-5c049c54b653)

By doing this, we combine the data from all months into one file, allowing us to analyze the entire dataset rather than working with multiple separate files. This is essential for performing comprehensive analysis across different time periods and ensuring consistency in the data.

#### Step 3 Inspecting the Dataset

After importing the dataset, it's important to verify its structure and understand the types of data it contains. We can do this using the info() function in pandas, which provides details about the dataset, such as the number of entries, column names, data types, and the presence of missing values.

![image](https://github.com/user-attachments/assets/03870af0-1154-45e5-bf7d-5958e4d5469d)

In the dataset, we found missing values represented as empty rows. To ensure the accuracy of our analysis, we decided to drop these empty rows using the dropna() method.
and we noticed that all the data types in the dataset were set as object. This is problematic because certain columns (such as numerical values for quantity and price) need to be transformed into appropriate data types (e.g., integers or floats) for proper analysis and calculations.
To address this, we will convert the relevant columns to their correct data types. For example, we need to convert the Quantity Ordered and Price Each columns to numeric types, and the Order Date column to a datetime type.

![image](https://github.com/user-attachments/assets/27ae9585-3bda-428c-9b67-561832146a51)

![image](https://github.com/user-attachments/assets/2b513391-9fdc-4387-89c7-7bb015fca95f)

#### Step 4: Analyzing the Data Answering the Business Questions
After cleaning and preparing our dataset, we can now move on to the core of our project: analyzing the sales data to extract meaningful insights.
In this section, we will answer a set of key business questions, such as:

- What was the best month for sales and how much was earned that month?

- What city had the highest number of sales?

- What time should advertisements be displayed to maximize customer purchases?

- Which product sold the most and why?

To answer the first question, we need to create a new column called Sales, which is the result of Quantity Ordered * Price Each. Then, we group by month and sum the total sales.

![image](https://github.com/user-attachments/assets/916a0f9b-cdb1-4fd6-8cd5-1130e5c0b7a1)
![image](https://github.com/user-attachments/assets/9c4b7aff-6238-44f9-ba03-cc4a0b885642)
![image](https://github.com/user-attachments/assets/e802a017-363b-4173-a5f8-1360f7718039)

### Visualization
![image](https://github.com/user-attachments/assets/1e3d08d5-f0e6-4335-901d-f83012c8a65b)

December emerged as the best-performing sales month in 2019, . This exceptional performance likely reflects heightened consumer spending during the holiday season, when gift purchases and year-end promotions typically drive sales peaks. The December revenue exceeded the monthly average by approximately 40%, demonstrating the significant impact of seasonal demand on business performance. This substantial earnings spike suggests that holiday marketing strategies, inventory planning, and promotional campaigns were particularly effective during this period. Companies can leverage this insight by intensifying their Q4 sales initiatives and ensuring optimal stock levels to maximize future December revenue opportunities.

#### What city had the highest number of sales?

![image](https://github.com/user-attachments/assets/2ae706f8-2329-483f-8148-89811ea46833)

![image](https://github.com/user-attachments/assets/12ceebee-2f96-4668-b2f2-4f7cb3ecf3bf)

### Visualization

![image](https://github.com/user-attachments/assets/43fa6a88-798c-42f3-b0e3-7f18ecd116d0)

The order distribution analysis reveals that San Francisco is the top-performing city, with 44,732 orders, likely driven by a tech-savvy population, strong digital infrastructure, and a high level of e-commerce adoption. Los Angeles follows with 29,605 orders, reflecting its large, diverse metropolitan market. Surprisingly, New York City ranks third with 24,876 orders, a relatively modest figure considering its population density, which suggests untapped market potential or operational inefficiencies. Mid-sized cities like Boston (19,934) and Atlanta (14,881) show moderate engagement, while Dallas, Seattle, Portland, and Austin trail with under 15,000 orders each—Austin registering the lowest with 9,905 orders. This stark contrast, especially between San Francisco and Austin, may result from uneven market penetration, regional supply chain advantages on the West Coast, or demographic differences in consumer behavior. These findings point to the need for targeted marketing strategies, customer engagement efforts, and supply chain assessments to strengthen performance in underperforming regions and maximize overall sales potential.

#### What time should advertisements be displayed to maximize customer purchases?

![image](https://github.com/user-attachments/assets/efa8d4c6-e0ac-4c8f-9d65-9b34c375c41a)

### Visualization 

![image](https://github.com/user-attachments/assets/a5b49a80-b635-4239-adf9-67365c35f25c)

To maximize customer purchases, advertisements should be strategically timed to align with peak transaction hours. The data reveals two prime windows for ad placements: midday (12:00-13:00) with 12,587 transactions and evening (19:00-20:00) with 12,905 transactions, making these the optimal times to capture high purchase intent. Strong secondary periods include mid-morning (10:00-11:00) and early evening (18:00-19:00), which show sustained activity levels above 10,000 transactions per hour. Morning hours from 8:00 onward demonstrate steady growth, peaking at 12,411 transactions by 11:00, while afternoon hours maintain consistently high volumes above 12,000 transactions between 12:00 and 14:00. By contrast, overnight hours (23:00-5:00) account for less than 7% of total daily transactions, representing poor ad value. For optimal results, advertisers should concentrate 70-75% of their budget during the twin peaks of midday and evening hours, when consumer purchasing behavior is most active, while using remaining resources to maintain visibility during the strong secondary periods that bookend these peaks. This timing strategy ensures maximum exposure during proven high-conversion periods while maintaining efficient ad spend allocation.

#### Which product sold the most and why?

![image](https://github.com/user-attachments/assets/6580428e-6596-4421-8586-b91a96ca02e6)

### Visualization 

![image](https://github.com/user-attachments/assets/5252c406-7514-483c-9f9f-7fea4971a850)

AAA Batteries (4-pack) emerged as the top-selling product with 31,017 units sold, outperforming all other items by a significant margin. This dominance stems from their universal utility across countless household devices, from remote controls to children's toys, creating consistent demand regardless of season or consumer demographics. The product's success is further amplified by its affordable price point, which eliminates typical purchasing hesitation and encourages impulse buys, along with its role as a natural complement to many electronics sold in the same marketplace. The broader trend of battery and charging-related products occupying the top four spots suggests customers prioritize essential, frequently replaced accessories over premium electronics, likely due to their everyday necessity and compatibility with multiple devices. This sales pattern indicates that practical, low-cost items with universal applications tend to outperform specialized, high-ticket products in this retail environment, highlighting the importance of maintaining strong inventory and strategic positioning for these high-demand commodity goods.


### Project N°2 HR Attrition Analysis 
  
#### Table of contents
- [Title](#title)
- [Description](#description)
- [Tools Used](#tools-used)
- [Data Source](#data-source)
- [Python Data Cleaning & Visualization](#python-data-cleaning-and-visualization)
- [Step 1: Importing Necessary Packages ](#step-1-importing-necessary-packages)
- [Step 2 Importing the Dataset ](#step-2-importing-the-dataset)
- [Step 3: Verifying the Dataset ](#step-3-verifying-the-dataset)
- [Step 4: Checking for Duplicates ](#step-4-checking-for-duplicates)
- [Step 5: Descriptive Statistics ](#step-5-descriptive-statistics)
- [Step 6: Distribution of Age](#step-6-distribution-of-age)
- [Step 7: Attrition Analysis](#step-7-attrition-analysis)
- [Step 8: Analysis of Employee Distribution and Attrition by gender ](#step-8-analysis-of-employee-distribution-and-attrition-by-gender)
- [Step 9: Analysis of Employee Distribution and Attrition by Department](#step-9-analysis-of-employee-distribution-and-attrition-by-department)
- [Step 10: Analysis of Employee Distribution and Attrition by Marital Status](#step-10-analysis-of-employee-distribution-and-attrition-by-marital-status)
- [Step 11: Attrition Analysis by Education Field](#step-11-attrition-analysis-by-education-field)
- [Step 12: Attrition Analysis by Stock Option Level](#step-12-attrition-analysis-by-stock-option-level)
- [Step 13: Attrition Analysis by Relationship Satisfaction](#step-13-attrition-analysis-by-relationship-satisfaction)
- [Step 14: Attrition Analysis by Job Satisfaction](#step-14-attrition-analysis-by-job-satisfaction)
- [HR Attrition Analysis Dashboard (Power BI)](#hr-attrition-analysis-dashboard-power-bi)
- [HR Attrition Analysis Dashboard by Male (Power BI)](#hr-attrition-analysis-dashboard-by-male)
- [HR Attrition Analysis Dashboard by Female (Power BI)](#hr-attrition-analysis-dashboard-by-female)


#### Title  
HR Attrition Analysis 

#### Description

This project focuses on analyzing employee attrition to help HR teams identify key drivers of employee turnover. Using an interactive dashboard, the project visualizes critical metrics such as attrition rates by department, age group, and job role, empowering decision-makers with actionable insights.

#### Tools Used 

- Python for data cleaning and visualisation
- Power BI for dashboard creation.

#### Data Source
The data used for this project is sourced from the [Kaggle HR Analytics Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset).

### Python Data Cleaning and Visualization 

#### Step 1 Importing Necessary Packages

The first step in any data analysis project is to import the necessary packages or libraries. These libraries provide the functions and tools needed to manipulate the data, perform computations, and create visualizations. Below is the code I used to import the required packages for this project:

![image](https://github.com/user-attachments/assets/2cb3f92b-eadf-43f4-8037-44612a090145)

#### Step 2 Importing the Dataset 
 
The next step is to import the dataset into our Python environment. This is done using the pandas library, which allows us to easily load and manipulate data. Below is the code I used to import the dataset and display the first few rows for a quick preview.


![image](https://github.com/user-attachments/assets/8cfd8fd7-1ee6-438e-a270-f38f56699f98)

##### output 

![image](https://github.com/user-attachments/assets/353dd663-09c2-4164-be01-4b6aafe51560)

#### Step 3 Verifying the Dataset 

After importing the dataset, it's important to verify its structure and understand the types of data it contains. We can do this using the info() function in pandas, which provides details about the dataset, such as the number of entries, column names, data types, and the presence of missing values.

![image](https://github.com/user-attachments/assets/b7709037-80c1-4d09-a208-b7440a32584a)

##### output 

![image](https://github.com/user-attachments/assets/6027d574-48d0-4e16-92cc-1abb4a55460c)

This output indicates that the dataset contains ***1470*** entries with no null values across all columns, which ensures data completeness. Additionally, the data types for each column are appropriate, with int64 for numerical variables and object for categorical variables. This suggests that the dataset is clean and ready for analysis, with no immediate need for data type corrections or null value handling.

#### Step 4 Checking for Duplicates 

In data analysis, it's crucial to check for duplicate entries, as they can skew your results. To ensure the integrity of the dataset, we use the duplicated() function to identify any duplicate rows.


![image](https://github.com/user-attachments/assets/23660a78-47e6-409c-bec7-cb44a708de89)

##### output 

![image](https://github.com/user-attachments/assets/21fec74f-d845-4ce8-93df-b5cb775d70b8)

This output  confirms that there are no duplicate rows in the dataset. This indicates that the data is unique and does not require any deduplication process, ensuring the integrity of the dataset for analysis.


##### "We have thoroughly verified the dataset, including checks for null values, duplicate rows, data types, unique identifiers, and potential inconsistencies. All aspects of the data are in good condition, with no issues requiring modification. The dataset is clean, complete, and ready for further analysis"

#### Step 5 Descriptive Statistics 

To better understand the dataset, I performed descriptive statistical analysis using the describe() function in pandas. This step provides a summary of the dataset's numerical columns, helping to identify key metrics like the mean, median, and standard deviation.

![image](https://github.com/user-attachments/assets/dc46e0c3-dc35-4107-b7e7-cc044e8f3046)

##### output 

![image](https://github.com/user-attachments/assets/65a405d7-f4be-4bc5-a1f4-b5db88ae84c2)

Descriptive statistics provide a comprehensive overview of a dataset's key characteristics, allowing us to understand its structure and tendencies.

we have :

- Mean: The average value, indicating the central point.
- Standard Deviation: The variability around the mean.
- Range (Min and Max): The span from the smallest to the largest value.
- Q1 : The First Quartile The value below which ***25%*** of the data falls.
- Q2 : The Second Quartile The middle value of the dataset when sorted. It divides the data into two equal halves.
- Q3 : The Third Quartile The value below which ***75%*** of the data falls.

#### Step 6 Distribution Of Age 

![image](https://github.com/user-attachments/assets/5783deb3-1d6a-4713-a40e-2b9f09aee4fa)

##### output

![image](https://github.com/user-attachments/assets/43fb0481-0ef6-4327-9646-b6fe04013f05)


#### Step 7 Attrition Analysis 

In this step, we analyze the Attrition column of the dataset to understand the distribution of employee attrition (whether employees left or stayed in the company).

![image](https://github.com/user-attachments/assets/fd15924a-eebb-46ad-be2e-2f2ca186698b)

##### output 

![image](https://github.com/user-attachments/assets/0ade1ee2-ba2c-47b3-86f9-9ddd7b3c92bc)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/55d9c60f-1d57-4b45-9171-cb947589b59f)

**YES**: means left

**NO**: means stayed

The Attrition Count indicates that out of the total ***1470*** employees in the dataset, ***1233*** employees stayed with the company (marked as 'No'), while ***237*** employees left the company (marked as 'Yes').

The Attrition Percentage reveals that approximately ***83.88%*** of the employees stayed, while about ***16.12%*** of employees left the company. This provides a clear picture of the employee retention rate, indicating that a relatively small proportion of employees decided to leave. However, it’s essential to explore the reasons behind the attrition. By analyzing various factors and variables (such as age, job satisfaction, work-life balance, etc.), we can identify the key drivers of employee turnover and gain valuable insights into areas that may need attention to reduce attrition



#### Step 8 Analysis of Employee Distribution and Attrition by gender

In this step, we analyze  Distribution of gender and the relationship between employee attrition and gender to determine if there are any gender-based patterns or differences in attrition rates.

![image](https://github.com/user-attachments/assets/46e84e99-0ba3-4107-b20a-134af06042a8)

##### output 

![image](https://github.com/user-attachments/assets/2b5cbda8-036d-4a74-beda-4d4f5e0734ed)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/23b887c7-8903-48b8-8a50-62622c78dcc3)

##### output 

![image](https://github.com/user-attachments/assets/fd45c331-5fcd-4879-b83a-9d1a2b7625ff)

This indicates that males constitute the majority of the workforce, while females represent a significant portion as well. Understanding gender distribution can be important for analyzing various factors, such as diversity, employee engagement, and attrition rates across different genders.

### Attrition by gender

![image](https://github.com/user-attachments/assets/703c80ed-88a8-4b88-9b06-11c80bf06092)

##### output 

![image](https://github.com/user-attachments/assets/8abb7f3b-47c5-4ed6-9a9b-3eef65196276)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/beff3170-0e22-4772-86f9-81ed7f0cf5d8)

##### output

![image](https://github.com/user-attachments/assets/a2b7bc27-fafd-4d5f-a4db-979702d75659)

#### The results provide a gender-specific analysis of attrition:

- Female Employees:

***85.20%*** of female employees stayed with the company, indicating a high retention rate among women.

Only ***14.80%*** of female employees left the company, reflecting a relatively low attrition rate.

- Male Employees:

***82.99%*** of male employees stayed with the company, which is slightly lower than the retention rate for female employees.

***17.01%*** of male employees left the company, indicating a higher attrition rate compared to females.

These results suggest that female employees tend to have a slightly higher retention rate than male employees in the company. The reason behind this difference could be explored further by analyzing factors such as job satisfaction, work environment, or other demographic and professional attributes. Understanding these dynamics can help the company address specific issues related to male attrition and improve overall employee retention

#### Step 9 Analysis of Employee Distribution and Attrition by Department

in this step we will explore the distribution of employees across various departments and analyze the attrition (employee turnover) rate within each department

![image](https://github.com/user-attachments/assets/51c18d67-a1fb-4c65-a63e-a3f70b7ac13b)

#### output

![image](https://github.com/user-attachments/assets/2aebedfd-a2ab-4d7e-9bc0-f261b1f73067)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/d8f44400-98de-4a68-9fca-ee76879a9c2e)

![image](https://github.com/user-attachments/assets/5d70d640-1e5a-43d8-af1a-cfe2431f41f0)

This distribution shows a clear dominance of the R&D department, followed by Sales, while HR has a relatively smaller representation. These proportions are crucial for understanding the scale of operations within each department and for further analyzing the attrition rates within these specific sectors.

### Attrition by department 

![image](https://github.com/user-attachments/assets/f3fd50a3-ad23-45f4-a0e0-093792b76a16)

#### output 

![image](https://github.com/user-attachments/assets/cb547943-edcd-48c0-8470-5fff290dc1af)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/8fe502b0-3dd2-4cf8-a7d9-d46bd0ea4371)

#### output 

![image](https://github.com/user-attachments/assets/cfb9ad77-ef17-44f5-8e17-2b7a65488e78)

The data shows that while Research & Development has the lowest attrition rate, Sales and Human Resources exhibit relatively higher levels of employee turnover.

#### Step 10 Analysis of Employee Distribution and Attrition by Marital Status 

In this step, we explore the marital status distribution of employees, calculating both the total number of employees in each marital status category and their corresponding percentages. Additionally, we analyze attrition rates based on marital status. By understanding the relationship between marital status and attrition, we can identify whether certain marital statuses correlate with higher or lower employee turnover. This information may help in making targeted interventions to improve retention across different employee groups.

![image](https://github.com/user-attachments/assets/03f38a5c-885d-46f5-b5ee-00cd6fe2c55a)

#### output 

![image](https://github.com/user-attachments/assets/2e4b8baa-395c-4c8b-9a03-5f1413ccd44b)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/55d546dd-4034-4128-bc7d-536ba357763e)

#### output 

![image](https://github.com/user-attachments/assets/41d2edf7-82f2-444e-802a-d130e720443f)

The distribution of marital status among employees shows that the majority are married (45.78%), followed by single employees (31.97%) and divorced employees (22.24%). This suggests that marital status is relatively balanced, with a larger portion of the workforce being married. The next step would be to analyze how attrition correlates with these marital status categories to determine if employees in certain marital statuses are more likely to leave the company.

### Attrition by Marital status

##### Here's a visualization

![image](https://github.com/user-attachments/assets/77831a34-89df-4abd-9f1a-af9186b298be)

#### output 

![image](https://github.com/user-attachments/assets/54aa07a8-9cb2-46ad-86c2-eba6466f282c)

This visualization shows the attrition distribution by marital status. Key insights from the charts:

1. ***Single Employees***: Among single employees, 25.5% have left the organization (attrition), while 74.5% have stayed. This is the highest attrition rate among the three groups.
2. ***Married Employees***: Only 12.5% of married employees have left the organization, with 87.5% staying. This indicates the lowest attrition rate.
3. ***Divorced Employees***: 10.1% of divorced employees have left, and 89.9% have stayed. This group also has a very low attrition rate, similar to married employees.µ

- Single employees seem to be more prone to attrition compared to married or divorced employees.
- Stability in employment appears higher among married and divorced groups. This trend could suggest that marital status influences employee retention.

#### Step 11 Attrition Analysis by Education Field

In this step, we analyze the distribution of employee attrition across different education fields.

![image](https://github.com/user-attachments/assets/af9e1770-d80d-4c39-a46c-2fc138caf0f1)

#### output 

![image](https://github.com/user-attachments/assets/eb338a5c-5740-4850-b961-8b6c1c48ce48)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/589ddf5b-26b5-4991-a9af-b18efc7652be)

#### output 

![image](https://github.com/user-attachments/assets/f1a997ad-4b71-4ae6-afa9-3e1cab188358)

 Human Resources and Technical Degree experience higher attrition rates, which may require further investigation into job satisfaction, opportunities for growth, or workplace conditions. On the other side, 
 Medical, Life Sciences, and "Other" fields show strong retention rates, reflecting a high level of employee satisfaction and stability.

#### Step 12 Attrition Analysis by Stock Option Level

In this step, we analyze employee attrition rates based on the Stock Option Level. First, we group the data by both the Stock Option Level and Attrition status to count the number of occurrences for each combination. Then, we calculate the percentage of employees who left (attrition) for each Stock Option Level by dividing the number of attritions by the total number of employees in each Stock Option Level. This allows us to gain insights into whether the Stock Option Level influences the likelihood of attrition. The results are displayed both in absolute terms (count) and as percentages.

![image](https://github.com/user-attachments/assets/23b23c9e-9d6f-44fa-ac57-aea76671ea9e)

#### output 

![image](https://github.com/user-attachments/assets/0c7fb02e-f597-4a17-98cb-67693ec9a0b9)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/f6f515ed-5a51-48c7-bb8d-f8ceea415053)

#### output 

![image](https://github.com/user-attachments/assets/b3e35236-8ad0-4186-853b-0ea8d4b891e6)

the output suggests that employees with higher stock option levels tend to have a lower likelihood of attrition, 

#### Step 13 Attrition Analysis by Relationship Satisfaction

In this step, we examine the relationship between employee attrition and their Relationship Satisfaction with the company

![image](https://github.com/user-attachments/assets/4844b6db-4818-479e-92d3-aa5ff212a40b)

#### output 

![image](https://github.com/user-attachments/assets/32be2970-2886-46af-a382-bbdd1dc96794)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/7573540f-920f-4cb0-b8f9-29aac3122235)

#### output 

![image](https://github.com/user-attachments/assets/2c78a1d1-7929-43ba-9c8f-f3c25dad95bb)

The analysis reveals that employees with varying levels of Relationship Satisfaction exhibit different attrition patterns. Employees with low satisfaction (level 1) show the highest attrition rate at 20.65%, while those with higher satisfaction levels (2, 3, and 4) consistently have lower attrition rates, hovering around 14-15%. This suggests that employees who are more satisfied with their relationships at work are less likely to leave, highlighting the importance of fostering positive work relationships to reduce turnover.

#### Step 14 Attrition Analysis by Job Satisfaction

In this step, we analyze employee attrition based on their Job Satisfaction levels. By examining how employees with different satisfaction levels (ranging from low to high satisfaction) relate to the likelihood of leaving the company, this analysis helps identify whether job satisfaction plays a significant role in attrition rates.

![image](https://github.com/user-attachments/assets/55597c16-2232-48c3-bf1d-2c2398073775)

#### output 

![image](https://github.com/user-attachments/assets/c68d986d-a6b8-4392-b98a-17450e610c92)

##### Here's a visualization

![image](https://github.com/user-attachments/assets/bd59ec89-ca6e-42d9-8d69-ad45ab420564)

#### output

![image](https://github.com/user-attachments/assets/37f14d81-5027-4de6-b70f-1af6b2772d76)

This analysis reveals the relationship between Job Satisfaction and employee attrition. Employees with lower job satisfaction (Job Satisfaction level 1) exhibit a higher rate of attrition, with nearly 23% leaving the company. As job satisfaction increases, the attrition rate steadily decreases, with employees at the highest satisfaction level (Job Satisfaction level 4) showing an attrition rate of just over 11%. This trend highlights the importance of improving job satisfaction to reduce turnover, as more satisfied employees are less likely to leave the organization.

### HR Attrition Analysis Dashboard Power Bi

Welcome to the HR Attrition Analysis Dashboard! This interactive dashboard provides valuable insights into employee attrition trends within the organization, helping HR and management teams understand patterns and make informed decisions to reduce turnover.

This dashboard visualizes key metrics and trends related to employee attrition, including factors such as department, tenure, stock option levels, relationship satisfaction, and more. By using Power BI's advanced filtering and visualization capabilities, users can explore different dimensions of the data, identify risk factors, and pinpoint areas that require attention. The goal is to empower decision-makers with actionable insights to improve employee retention strategies and enhance the overall work environment.

### Overall dashboard

![image](https://github.com/user-attachments/assets/419e75b8-2b04-4789-891e-36acb5d31478)

The HR Attrition Analytics Dashboard is a comprehensive tool designed to provide valuable insights into employee turnover and workforce dynamics within the organization. At its core, the dashboard displays five essential metrics that give an immediate overview of the organization's workforce status: a total employee count of 1,470, an attrition count of 237 employees who have left, resulting in an attrition rate of 16.12%, with 1,233 active employees remaining, and an average employee age of 36.92 years.

The dashboard offers detailed breakdowns of attrition across various dimensions. In terms of departmental analysis, Research & Development has experienced the highest turnover with 133 departures (56.12% of total attrition), followed by Sales with 92 departures (38.82%), and Human Resources with 12 departures (5.06%). When examining educational backgrounds, Life Sciences leads with 89 departures, followed by Medical with 63, Marketing with 35, and Technical Degrees with 32, while other fields show lower numbers.

Age-based analysis is presented through a histogram, revealing patterns in turnover across different age groups, with notable concentrations in early career years. The dashboard also shows a clear correlation between stock options and retention, with higher attrition among employees holding fewer stock options, demonstrating the impact of equity-based compensation on retention.

Employee satisfaction is measured through relationship satisfaction levels on a 1-4 scale, with notable peaks at level 3 (71 employees) and level 4 (64 employees). The dashboard provides a detailed job satisfaction breakdown across various roles, including Sales Representatives, Research Directors, Manufacturing Directors, Managers, Laboratory Technicians, Human Resources staff, and Healthcare Representatives.

The dashboard's interactive features allow for dynamic filtering by department, marital status, and gender, enabling more targeted analysis. This functionality helps in identifying specific patterns and trends within different employee segments.

From a strategic perspective, this dashboard serves as a crucial tool for workforce planning, helping management develop targeted retention strategies, assess compensation effectiveness, understand demographic impacts on turnover, evaluate departmental management effectiveness, and monitor satisfaction metrics. It enables data-driven decision-making in areas such as retention program development, compensation strategy refinement, organizational development initiatives, and human capital risk management.

This comprehensive view of workforce dynamics helps organizations proactively address retention challenges, optimize human resource strategies, and maintain a stable and satisfied workforce. The insights provided can guide both immediate interventions and long-term strategic planning in human resource management.

### HR Attrition Analysis Dashboard by male

![image](https://github.com/user-attachments/assets/318a496b-c384-4627-a807-9be3cfc7fdf3)

### HR Attrition Analysis Dashboard by female

![image](https://github.com/user-attachments/assets/7ed8b656-4e5b-4337-b1b8-5032b4c95035)




### Project N°3 In Progress  
*Details will be added soon.*
















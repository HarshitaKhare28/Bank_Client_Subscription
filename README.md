# Bank_Client_Subscription
## Description
Exploratory data analysis on the bank-client subscriptions from the file Bank-additional-full.csv.
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls.
Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.
# Details
## Data Loading
Created a dataset in form of a csv file, read it using ‘csv_read()’ and
assigned it to a variable ‘df’.
The csv file was uploaded to github and accessed via link for smoother
functioning of the program.
The csv file contains data related with direct marketing campaigns of a
Portuguese banking institution, a total of 41188 entries and 20 inputs
## Data Description and Inspection
 Display the first 10 rows of the dataset to get a glimpse of its structure.
(df.head(10))
 Check the size of the dataset and inspect the last 5 rows. (df.shape(),
df.tail(5))
 Examine basic statistics and information about the dataset, such as mean,
standard deviation, and data types. (df.describe(), df.info())
 Obtain general information about the dataset, including the presence of
null values. (df.isnull())
## Grouping and Aggregation
aim to understand the relationship between marital status and the
average age of clients
 The process involves grouping the data based on marital status and
calculating the mean age within each group.
 Contributes to a comprehensive understanding of how certain
demographic factors, such as marital status, may influence the average
age of clients in the context of the dataset.
## Filtering and Sorting
 Filtering the dataset based on specific criteria and sorting the filtered data
to gain insights into particular patterns or characteristics.
 Once the data is filtered, sort it based on a chosen column, such as 'age,' to
arrange the results in a specific order.
 Insights gained from this step may provide valuable information about
specific segments of the dataset.
## Visualizations
 The goal is to create visual representations of the data to better
understand its distribution, patterns, and relationships.
 Identify categorical columns in the dataset, excluding the target variable.
 For each categorical column, create a count plot (bar chart) to visualize the
distribution of categories.
 Analyze the count plots to understand the distribution of categorical
variables.
## Insightful Visualizations
 The objective is to create visualizations that offer deeper insights into
specific aspects of the data, providing a more nuanced understanding of
patterns and relationships.
 Sankey Diagram: to visualize the flow and relationships between different
factors related to client subscription.
 It is particularly useful for illustrating the connections between different
categories and understanding the distribution of client subscriptions.
 Insights gained:
1. we have very less number of Individuals who are subscribing for
term deposit.
2. Majority of our dataset has people from the age group of 25-35,
followed by 35-45
 Sunbrust chart: particularly effective for visualizing hierarchical data with
multiple categorical levels
 Utilize a visualization library (i.e. Plotly Express) to create a Sunburst Chart
with the prepared data.
 Insights gained:
1. Married people are more likely to get a term deposit subscription
## Correlation Analysis
 Analyzing the correlation between numerical features in the dataset to
understand relationships and dependencies.
 Utilize a heatmap to represent correlation values, with colors indicating
the degree of correlation.
 BoxPlot: It allows to compactly visualize the main characteristics of the
feature distribution (the median, lower and upper quartile, minimal and
maximum, outliers (a data point that differs significantly from other observations).
 Insights gained:
1. Unmarried people are on average younger than divorced and
married ones
2. For the last two groups, there is an outlier zone over 70 years old,
and for unmarried - over 50.
## Data Cleaning and Manipulation
 The objective is to prepare the data for machine learning tasks or further
analysis through various cleaning and manipulation techniques.
 Implement outlier removal techniques to eliminate extreme values that
could impact analysis or model performance.
 Convert categorical columns into numerical format using one-hot
encoding. (One hot encoding is a technique that is used to represent categorical
variables as numerical values in a machine learning model.) (pd.get_dummies())
 Note: In our example, as we will not be running a machine learning model,
we have only performed few basic data manipulation techniques generally
done before running a model.
# Observed Outcome:
Through the analysis we have made the following conclusions:
 Data analysis on the basis of job factor shows that people who are retired
are more likely to take a term deposit than others and blue-collar workers
are less likely to take a term deposit than others.
 Our analysis on the factor of marital status of people shows that the
probability of single people subscribing is more.
 Also it shows that people who didn’t take a loan from the bank will apply
for term deposits.

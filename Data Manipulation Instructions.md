# Data Manipulation Instructions
In this study, we work with open data on [Popular Baby Names](https://www.ssa.gov/oact/babynames/limits.html) made by the United States Social Security Administration (SSA).  

We will explore reading in multiple raw data files in jupyter, merging them into one DataFrame, subsetting desired portions of the data, creating new variable metrics, and visualizing results in python.

## Load and preview the raw data
Use the '.read_csv()' method to access the first .txt file of baby names in 1880. We several names from the data that year (n>=5), with 3 variables: the name, the sex of the baby, and the birth count for that name.

## Aggregate and explore the data 
After we are familiar with the content and format of the original data, we can manipulate the data using Series and DataFrame method. To learn more detail about these powerful build-in functions in Pandas, always refer to [API references](https://pandas.pydata.org/pandas-docs/stable/reference/index.html)!

## Creat new variable metrics and data subset
Here we add the column of proportions ('prop') to our DataFrame. The proportions will be the number of births out of each total births grouped by year and sex. Then we divide the births by the sum of births in the grouping, and return the number.  

With this new DataFrame, we now will subset the top 1000 names by birth in each year and sex grouping. Define a new method, 'get_top1000()', and which sorts the births in descending order, and returns the first 1000 entries.

## Visualize the data
With the full dataset and Top 1,000 dataset in hand, we can start analyzing various naming trends of interest. First, we split the Top 1,000 names into the boy and girl portions. And then a pivot table is of the total number of births by year and name formed and plotted for some names in the dataframe.

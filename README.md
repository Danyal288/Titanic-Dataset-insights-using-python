# Titanic-Dataset-insights-using-python
Performing exploratory data analysis **(EDA)** on the Titanic Dataset using python and visualized the results.

Its a data science project completed on python jupiter notebook. I use Titanic Dataset from kaggle. 

# Loading and cleaning
I have used the numpy, panda, matplotli.pyplt and seaborn pakages of python.

1-imported all the pakages using *imort* command.

2-uploaded the dataset using *py.read_scv*.

3-find any null value using * .isna().usm()* command.

4-Then dropped the unnecessary columns using *.drop(Columns=[column_name], errors=ignore)*.

5- I needed the data in int from so I have to convert *Sex* column to int so I used  *df['Sex'].map({'male': 1, 'female': 0})* command

This data set has some major and minor erros.
There are some duplicate, which has been removed
In **Age** column, there are values many values that are missing. I used the fill method for this set. The statistical methods are not giving the desired results.
There was a outliner in **Fare** coloum that has been removed.

# Visualization
for this project I have created a *bar chart* to see number of age.using seaborn pakaged.

**sns.histplot(df['Age'], bins=25,multiple = "dodge")**

I also draw a coorelation matrix for this to see the coorelation of sets. it is alos seaborn pakage.

**sns.heatmap(df.corr(), vmin=-1, annot=True, cmap='coolwarm')**


# Insights/Findings
***There are couple of things that I have found.***

1- *Using heat map I have found a coorelation between Fare and Survived.* .  The positive relation suggest that if someone has paid more money to travel there are chances of serival of that person.

2- There is a negative coorelation between survived and Age!.   It means the younger people have more chances of servial in titanic.

 

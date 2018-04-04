---
title: Explore the data
description: >-
  Before any serious analytics can begin, it is important to understand your data better. We do this by performing Exploratory Data Analysis (EDA). A few of the available EDA methods will be covered in this chapter.


---
## Let's get some info!

```yaml
type: NormalExercise
lang: python
xp: 100
skills: 2
key: 5f798c6519
```

We will begin by getting some very broad information about the DataFrame `df`. For this purpose you will use the `info()` method.

After you submit the solution, take some time to read the success message that will help you interpret the results.

`@instructions`
Use the `info()` method on `df`


`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
```
`@sample_code`
```{python}
#Your code below
df.____()
```
`@solution`
```{python}
df.info()
```
`@sct`
```{python}
Ex().has_equal_ast()
success_msg("Success! You can see that the DataFrame has 110 rows of data and 6 columns. Furthermore, you can see the column names and the variable types that populate them.")
```





---
## Describe the data

```yaml
type: NormalExercise
lang: python
xp: 100
skills: 2
key: ff0ef50ee7
```

The `info()` method has given you some high-level insight into the dataset as a whole.

What about some statistical description of the individual columns? For this purpose we will use the `describe()`method.

This time you will use a variable to store the code. A variable is like a container that converts lengthy code into a short character string. 

Make sure you print the variable and take some time to interpret the output.

`@instructions`
1) Use the `describe()` method on `df`

2) Assign your code to a variable `description`

3) Print out the variable `description`


`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
```
`@sample_code`
```{python}
#Your code below
____ = df.____()

#Print the variable below
print(____)
```
`@solution`
```{python}
#Your code below
description = df.describe()

#Print the variable below
print(description)
```
`@sct`
```{python}
Ex().has_equal_ast()
success_msg("Wow, you just received a lot of useful information with a single `describe()` method!")
```





---
## Visualise the data

```yaml
type: NormalExercise
lang: python
xp: 100
skills: 2
key: 0a8799887e
```

Statistical analysis is great, but sometimes a visualization can be an extremely powerful tool to understand the data quickly and effectively. For this purpose you will import an new library called `matplotlib`.

We will focus on understanding the distributions of our data by creating a histogram. This will help your statistical analysis in the upcoming chapter. 

After you submit the exercises, let's take some time to interpret the results.

`@instructions`
1) Import the `matplotlib.pyplot` library as `plt`

2) Create a histogram of the `age` variable by using `hist`

3) Create a histogram of the `lifetime_value` variable by using `hist`

4) Display the histogram by using `plt.show()`

`@hint`


`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/e8c7de0372cfe29b1be7bad2b16e28e2e9a56d01/mars_data.csv')
```
`@sample_code`
```{python}
#Import the required modules
import matplotlib.pyplot as ____

#Create a histogram to show the distribution of age variable
df['____'].plot.____()
plt.show()

#Create a histogram to show the distribution of lifetime value variable 
df['____'].plot.____()
____
```
`@solution`
```{python}
#Import the required modules
import matplotlib.pyplot as plt

#Create a histogram to show the distribution of age variable
df['age'].plot.hist()
plt.show()

#Create a histogram to show the distribution of lifetime value variable 
df['lifetime_value'].plot.hist()
plt.show()
```
`@sct`
```{python}
Ex().has_equal_ast()
success_msg("Great work! Note that your data is skewed. We will have to do something about this in the future exercises")
```


---
## Bring it all together

```yaml
type: NormalExercise
lang: python
xp: 100
skills: 2
key: 1f72e72c18
```

Well done! Now you have a much better understanding of the Mars data. You achieved this by, firstly, having a high-level overview with the `info()` method. Then you explored the statistical features of the columns by using `describe()`. Finally, you visually examined the distribution of the values across multiple variables. 

Remember, you found that the both, `age` and `lifetime_value` columns are skewed. This means that you will have to transform the values of these columns to effectively apply statistical methods. You will learn more about this in the next chapter.

`@instructions`
Click `Submit Answer` once you are ready to proceed!

`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/e8c7de0372cfe29b1be7bad2b16e28e2e9a56d01/mars_data.csv')
```
`@sample_code`
```{python}
import matplotlib.pyplot as plt

df.info()

df.describe()

df['age'].plot.hist()
plt.show()

df['lifetime_value'].plot.hist()
plt.show()
```
`@solution`
```{python}
import matplotlib.pyplot as plt

df.info()

df.describe()

df['age'].plot.hist()
plt.show()

df['lifetime_value'].plot.hist()
plt.show()
```
`@sct`
```{python}
Ex().has_equal_ast()
success_msg("Let's march on to the final chapter!")





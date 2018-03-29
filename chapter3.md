---
title       : Analyse the data
description : In this chapter you will work to do the heavy lifting analysis that your manager has asked for.
---
## Find the value sum of a column

```yaml
type: NormalExercise
key: 108d33a707
lang: python
xp: 100
skills: 2
```
Now that you are familiar with the data, you can finally start exploring it in depth. 

Your manager has asked to find the total value of all the transactions that took place during the day. You can do this by using the `.sum()` method on the `lifetime_value` column. 

`@instructions`

1) Select the `lifetime_value` column of `df`

2) Apply the `.sum()` method

3) Assign the calculation to the variable `total_value`

4) Print the results


`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
```

`@sample_code`
```{python}
#Calculate the total value
____ = df['____'].____()

#Print out the results
print(____)
```

`@solution`
```{python}
total_value = 22005
```

`@sct`
```{python}
test_object('total_value')
success_msg("Good work! You can now report a profit of $22005 for the day now!")
```

---
## Find correlation between two variables

```yaml
type: NormalExercise
key: b8cf4b8501
lang: python
xp: 100
skills: 2
```
Your manager is convinced there is positive correlation between a customer's age and their lifetime value. This means that the indipendent variable of age influences the dependent variable of profit. In other words, the older the cusotmer, the more profit the bank receives. This could be for a viarety of reasons and your task is to explore this hypothesis further. 

We will use the `corr()` pandas function to see if your manager is right. 

`@instructions`
1) Use the `corr()` function to find the correlation between `age` and `lifetime_value`

2) Assign the code to a variable `correlation`

3) Print the new variable


`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
```

`@sample_code`
```{python}
#Find the correlation between the two variables
correlation = df['age'].___(df['lifetime_value'])

#Print out the results
print(_____)

```

`@solution`
```{python}
#Find the correlation between the two variables
correlation = df['age'].corr(df['lifetime_value'])

#Print out the results
print(correlation)
```

`@sct`
```{python}
test_object('total_value')
success_msg("Looks like your manager's intuition was right and now you have some empyrical evidence to support it!)
```

---
## Transform the data

```yaml
type: NormalExercise
key: 7e71720519
lang: python
xp: 100
skills: 2
```


`@instructions`

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}

```

`@sct`
```{python}

```

---
## Find correlation between transformed variables

```yaml
type: NormalExercise
key: a97d1d137c
lang: python
xp: 100
skills: 2
```


`@instructions`

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}

```

`@sct`
```{python}

```

---
## Visualise the correlations

```yaml
type: NormalExercise
key: 1d3c536bd7
lang: python
xp: 100
skills: 2
```


`@instructions`

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}

```

`@sct`
```{python}

```
---
## Bring it all together

```yaml
type: NormalExercise
key: efa8b20bb4
lang: python
xp: 100
skills: 2
```


`@instructions`

`@hint`

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}

```

`@sct`
```{python}

```

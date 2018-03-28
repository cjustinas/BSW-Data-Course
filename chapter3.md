---
title       : Analysing the data
description : 
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

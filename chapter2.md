---
title       : Explore the data
description : Before any serious analysis can begin, it is important to understand your data. We do this by perfomring Exploratory Data Anlysis (EDA). A few of EDA methods will be covered in this chapter.
---
## Let's get some info! 

```yaml
type: NormalExercise
key: 5f798c6519
lang: python
xp: 100
skills: 2
```
We will begin by getting some very braod infromation about the DataFrame `df`. For this purpose you will use the `info()` method.

Aftet you submit the solution, take some time to read the success message that will help you interpret the results.

`@instructions`

Use the `info()` method on `df`

`@pre_exercise_code`
```
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
```
`@sample_code`
```{python}
#Your code below
df.____()

```

`@solution`
```
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
key: ff0ef50ee7
lang: python
xp: 100
skills: 2
```
The `info()` method has given you some high-level insight into the dataset as a whole.

What about some more statistical description of the individual columns? For this purpose we will use the `describe()`method.

`@instructions`

Use the `describe()` method on `df`

`@hint`

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
#Your code below
df.describe()
```

`@sct`
```{python}
Ex().has_equal_ast()
```


---
## Explore a single column

Wow, you just received a lot of useful information with a single `describe()` method! 

Hold on... on second thought something is not right here. If the maximum age of the person in the dataset is 75, this means that they had to be born in the year 1985 - well before the first colonies were established, so their home planet cannot be Mars. 

We need to find a way to determine the maximum age for 

```yaml
type: NormalExercise
key: 7875e652d6
lang: python
xp: 100
skills: 2
```


`@instructions`

`@hint`

`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
```

`@sample_code`
```{python}
df.____('home_planet').____()['age']
```

`@solution`
```{python}
df.groupby('home_planet').max()['age']
```

`@sct`
```{python}

```

---
## <<<New Exercise>>>

```yaml
type: NormalExercise
key: 0a8799887e
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
#Import the required modules
import matplotlib.pyplot as plt

```

`@solution`
```{python}
#Import the visaulisaton library
import matplotlib.pyplot as plt

#Visaulise 

```

`@sct`
```{python}

```
---
## Bring it all together

```yaml
type: NormalExercise
key: 1f72e72c18
lang: python
xp: 100
skills: 2
```

Well done! You have 

`@instructions`

`@hint`

`@pre_exercise_code`
```
import pandas as pd

```

`@sample_code`
```
df.info()

df.describe()

```

`@solution`
```{python}

```

`@sct`
```{python}

```

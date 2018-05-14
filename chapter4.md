---
title       : Introduction to Machine Learning
description : In this final chapter you will get a brief in
---
## Import libraries for Machine Learning

```yaml
type: NormalExercise
key: 8a8f6f6a7c
lang: python
xp: 100
skills: 2
```


`@instructions`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

# Import function to devide your data into training and learning parts
from sklearn.cross_validation import train_test_split

# Import the Decision Tree algorythm
from sklearn.____ import ____

# Import function to test the accuracy of your prediction
from ____.____ import ____

```

`@solution`
```{python}
# Import function to devide your data into training and learning parts
from sklearn.cross_validation import train_test_split

# Import the Decision Tree algorythm
from sklearn.tree import DecisionTreeClassifier 

# Import function to test the accuracy of your prediction
from sklearn.metrics import accuracy_score

```

`@sct`
```{python}
Ex().has_equal_ast()
success_msg("Good work!")
```


---
## Separate the dependent variable

```yaml
type: NormalExercise
key: 1aa751294c
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
x = df.drop(['home_planet'])

y= df['home_planet'])

```

`@sct`
```{python}

```

---
## Split your data 

```yaml
type: NormalExercise
key: 6c98c363ad
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

x_train, x_test, y_train, y_test = train_test_split(x,y,test_size=0.2)
```

`@sct`
```{python}

```
---
## Create and run a simple Decission Tree model

```yaml
type: NormalExercise
key: fa17f9a513
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
dt = DecisionTreeClassifier(random_state=42)


dt.fit(x_train, y_train)
```

`@sct`
```{python}

```

---
## Test your model

```yaml
type: NormalExercise
key: ebb2499832
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
# Make predictions using the model you developed
y_dt = dt.predict(x_test)

# Test the accuracy of your model
accuracy_score(y_test,y_dt)
```

`@sct`
```{python}

```

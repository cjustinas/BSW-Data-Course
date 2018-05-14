---
title       : Introduction to Machine Learning
description : In this final chapter you will get a brief introduction to 
---
## Import libraries for Machine Learning

```yaml
type: NormalExercise
key: 8a8f6f6a7c
lang: python
xp: 100
skills: 2
```
Machine Learning is a complex and difficult science that takes years to master. Luckily 


`@instructions`
1) Select the `tree` module from the sklearn library and import the `DecissionTreeClassifier`

2) Select the `metrics` module from the `sklearn` library and import `accuracy_score`

The code to import the `train_test_split` functions has already been writen for you. 

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

# Import function to devide your data into training and learning parts from the cross_validation module of sklearn library
from sklearn.cross_validation import train_test_split

# Import the Decision Tree algorythm from the tree module
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
success_msg("Now you are ready to kick things off, good work!")
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
The first task is to devide your data into two sets: one containing the dependent varaible that you want to predict, the other containing the features that will be used to predict the class of the dependent variable. 

`@instructions`
1) Use the `drop` method on your data to delete the `home_planet` column. This will be assigned to the variable `x`

2) Select the `home_planet` column only and assign it to the variable `y`


`@pre_exercise_code`
```{python}
import pandas as pd
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')

```

`@sample_code`
```{python}
#Keep all columns except the home_planet one
x = df.drop(['____'])

#Select the home_planet column only
____ = df['home_planet'])

#Print the content of y
print(y)

```

`@solution`
```{python}
#Keep all columns except the home_planet one
x = df.drop(['home_planet'])

#Select the home_planet column only
y = df['home_planet'])

#Print the content of y
print(y)

```

`@sct`
```{python}
Ex().has_equal_ast()
success_msg("Good job!")
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
The next step is to split your data into a training and testing sets.

This means that your model will take the training features x 

`@instructions`

`@pre_exercise_code`
```{python}
import pandas as pd
from sklearn.cross_validation import train_test_split
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')

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
import pandas as pd
from sklearn.cross_validation import train_test_split
from sklearn.tree import DecisionTreeClassifier 
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
x = df.drop(['home_planet'])
y = df['home_planet'])
x_train, x_test, y_train, y_test = train_test_split(x,y,test_size=0.2)
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
Now that you have a model ready, you need to assess how well it works!

`@instructions`



`@pre_exercise_code`
```{python}
import pandas as pd
from sklearn.cross_validation import train_test_split
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score
df = pd.read_csv('https://assets.datacamp.com/production/repositories/2588/datasets/73d9f6626d0059203da53d733f5f781c4c9aed32/mars_data.csv')
x = df.drop(['home_planet'])
y = df['home_planet'])
x_train, x_test, y_train, y_test = train_test_split(x,y,test_size=0.2)
dt = DecisionTreeClassifier(random_state=42)
dt.fit(x_train, y_train)

```

`@sample_code`
```{python}
# Make predictions using the model you developed
predictions = dt.____(x_test)

# Test the accuracy of your model
____(y_test,predictions)

```

`@solution`
```{python}
# Make predictions using the model you developed
predictions = dt.predict(x_test)

# Test the accuracy of your model
accuracy_score(y_test,predictions)
```

`@sct`
```{python}

```

---
## Bring it all together

```yaml
type: NormalExercise
key: 1ee398e3ac
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

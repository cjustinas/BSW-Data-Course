---
title: Getting started
description: In this chapter you will learn how to kick off your data analysis project. This includes equiping your working environment with powerful libraries, importing the data you want to analyse and checking if the data import has been succesful.
---
## Import the required libraries

```yaml
type: NormalExercise
lang: python
xp: 100
skills: 2
key: 286ddf980c
```
`Libraries` are collections of code that have been wirtten by other developers and packaged for anyone to use.

Imagine libraries as tools for building a house - you would not make your own hammer, nails and bricks, but rather buy these items in a shop. Similarly, libraries equip you with useful code that can be easily reused. For free! 

Two of the most useful libraries are:

`pandas - for data manipulation and analysis`

`numpy - for working with data arrays`

`@instructions`

Import `pandas` library and name it `pd` for ease of use. 

The code to import the `numpy` library has already been written for you as an example.

`@pre_exercise_code`
```
```

`@sample_code`
```
#Import numpy library
import numpy as np

#Import pandas library
import ____ as ____
```

`@solution`
```
#Import numpy library
import numpy as np

#Import pandas library
import pandas as pd
```

`@sct`
```
test_import("pandas", same_as = True)
```
---
## Import the data

```yaml
type: NormalExercise
key: 56c6ebec11
lang: python
xp: 100
skills: 2
```
Now that you have imported `pandas` library, we can focus on acquiring the data. This means pointing pandas to a data source, so it can transform it into a `Data Frame`. In very broad terms a Data Frame is simply a data structure with rows and columns or observations and variables (you can think of it as a spreadsheet).

Pandas can import data from a variety of sources that include text files, databases, APIs and so on. For this particular project we will import an Excel file. 

`@instructions`

1) Use `pd.read_excel()` to tell Python you want to import an Excel file.

2) Make sure you include the filename `AAA.xlsx`

3) Assign the code above to a variable `df` (abreviation of Data Frame)

`@hint`

`@pre_exercise_code`
```
import pandas as pd

```

`@sample_code`
```
____ = pd.____(____)

```

`@solution`
```
df = pd.read_csv()

```

`@sct`
```
test_object("df")

```

---
## Check your data

```yaml
type: NormalExercise
key: 713861b8dd
lang: python
xp: 100
skills: 2
```
Congratulations! You have just imported your data...

...or have you? To view and check your data we will use the `head()` and `tail()` methods.

`@instructions`

Use `tail()` method on the df object and specify the parameter of `10` inside the brackets to view the last 10 rows of the Data Frame.

The `head()` method has been writen for you as an exmaple (it returns 5 rows of data if you do not specify a number in the brakcets).

`@pre_exercise_code`
```
import pandas as pd 

```
`@sample_code`
```
#Check the first 5 rows of the DataFrame
df.head()

#Check the last 10 rows of the DataFrame
df.____(____)
```

`@solution`
```{python}
#Check the first 5 rows of the DataFrame

df.head()

#Check the last 10 rows of the DataFrame

df.tail(10)
```

`@sct`
```{python}

```
---
## Bring it all together

```yaml
type: NormalExercise
key: 689f678c19
lang: python
xp: 100
skills: 2
```
You have made good progress so far. Not only have you learned about the importance of labraries, but also imported data required for the upcoming analysis and cheked if the import has been succesful. At this rate you will become an expierenced data analyst in no time!

We also briefly touched upon variables by defining `df`. But more on that in the upcoming exercises...

For now, review the glorious code you have writen.

`@instructions`

Click `Submit Answer` once you are ready to proceed!

`@pre_exercise_code`
```{python}

```

`@sample_code`
```
import pandas as pd

df = pd.read_csv('AAA.xlsx')

df.head()

```

`@solution`
```{python}

```

`@sct`
```{python}

```

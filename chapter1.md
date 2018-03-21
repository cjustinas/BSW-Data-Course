---
title: Getting started
description: In this chapter you will learn how to kick off your data analysis project.


---
## Import libraries

```yaml
type: NormalExercise
lang: python
xp: 100
skills: 2
key: 286ddf980c
```
Imagine libraries as tools for building a house - you would not make your own hammer, nails and bricks, but rather buy these items in a shop. Similarly, libraries equip you with useful code that can be easily reused. For free! 

Two of the most useful libraries are:

`pandas - for data manipulation and analysis`

`numpy - for working with data arrays`

`@instructions`

Import `pandas` library and name it `pd` for ease of use. The code to import the `numpy` library has already been written for you as an example.

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
```{python}

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



`@instructions`

1) Use pd.read_excel()

2) S

`@hint`

`@pre_exercise_code`
```
import pandas as pd

```

`@sample_code`
```
df = pd.____(____)

```

`@solution`
```
df = pd.read_csv()

```

`@sct`
```{python}

```

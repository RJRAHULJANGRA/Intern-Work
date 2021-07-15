# BOX PLOT

It is an another way to represent the data graphically , which basically helps us to measure that how well distributed the data in a dataset is . It displays the distribution of data in 5 number summary as follows:

1. Minimum
2. First Quartile (Q1 - 25th Percentile)
3. Median (Mid-value)
4. Third Quartile(Q3- 75th Percentile)
5. Maximum 

It can also tell you if your data is symmetrical, how tightly your data is grouped, and if and how your data is skewed.

# FUNCTIONS OF BOX PLOT

- Tell you the values of outliers .
- Identify if data is symmetrical .
- Determine how tightly data is grouped .
- See if your data is skewed

### _OUTLIERS_

A value that "lies outside" (is much smaller or larger than) most of the other values in a set of data. For example in the scores 25,29,3,32,85,33,27,28 both 3 and 85 are "outliers".

# BOX PLOT CHART


```python
#importing the required liabraries

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
```


```python
data= np.array([40,50,60,70,80,90,100,110,120,2,190])
```


```python
data
```




    array([ 40,  50,  60,  70,  80,  90, 100, 110, 120,   2, 190])



Syntax:
matplotlib.pyplot.boxplot(x, notch=None, sym=None, vert=None, whis=None, positions=None, widths=None, patch_artist=None, bootstrap=None, usermedians=None, conf_intervals=None, meanline=None, showmeans=None, showcaps=None, showbox=None, showfliers=None, boxprops=None, labels=None, flierprops=None, medianprops=None, meanprops=None, capprops=None, whiskerprops=None, manage_ticks=True, autorange=False, zorder=None, data=None)
18.

plt.boxplot(data)

plt.show()

# **PLOTTING THE BOX PLOT CHART**


```python
plt.boxplot(data)
plt.show()
```


    
![png](output_12_0.png)
    


# WORKING WITH IMAGES

There are different ways of Reading/inserting and working with images .

1. We can import the Pillow(PIL) liabrary to work with images.

# Opening the image


```python
from PIL import Image
```


```python
DS= Image.open('datascience.jpg')
```


```python
DS
```




    
![png](output_19_0.png)
    




```python
DS.size
```




    (500, 282)




```python
Width= 500
Height= 282
```


```python
DS.filename
```




    'datascience.jpg'




```python
DS.format_description
```




    'JPEG (ISO 10918)'



# Cropping the image


```python
DS.crop((0,0,300,200))
```




    
![png](output_25_0.png)
    



2. we can directly insert the image in the notebook from 'EDIT' tab and select the "insert image" option (remember that cell must be in markdown mode.)


```python

```

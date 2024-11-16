# EXNO5APPDS

# AIM:

      To implement Dashboards creation with Plotly and Dash using python.
      

# About Dash and Plotly tools:

Dash is a Python framework for building analytical web applications. Dash helps in building responsive web dashboards that is good to look at and is very fast without the need to understand complex front-end frameworks or languages such as HTML, CSS, JavaScript. Let’s build our first web dashboard using Dash.

Plotly library in Python is an open-source library that can be used for data visualization and understanding data simply and easily. Plotly supports various types of plots like line charts, scatter plots, histograms, box plots, etc.


# ALGORITHM:

Step 1: Import Necessary Library like dash and plotly.

Step 2: Load the dataset.

Step 3: Add dropdown using layout function and include the necessary options.

Step 4: Display the necessary visualization tools and include the necessary parameters.

Step 5: Display the output.


# CODING AND OUTPUT:
### NAME : MAMTHA I
### REG NO : 212222230076
```Python
import dash
from dash import dcc, html
from dash.dependencies import Input,Output
import plotly.express as px
import pandas as pd
import plotly.graph_objects as px
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = sns.load_dataset('tips')
```
```Python
import plotly.express as px
df = px.data.tips()
fig = px.scatter_3d(df, x='total_bill', y='sex', z='tip', color='day', size='total_bill', symbol='time')
fig.show()
```
![image](https://github.com/user-attachments/assets/23b91c93-293d-4631-9fc5-8f8834241426)


![image](https://github.com/user-attachments/assets/64af9a8a-5d16-447c-8277-eb7aff2e4912)

```Python
import plotly.express as px
df=px.data.tips()
fig = px.bar(df, x='day',y='total_bill',color='sex',facet_row='time',facet_col='sex')
fig.show()

```

![image](https://github.com/user-attachments/assets/808f2c57-6237-4150-b215-21dced2624c8)

```Python
import plotly.express as px
df=px.data.tips()
fig = px.histogram(df, x='total_bill',color='sex',nbins=50,histnorm='percent',barmode='overlay')
fig.show()
```

![image](https://github.com/user-attachments/assets/c6f0b81d-8bbe-4af0-a8e1-55bb8d9fa2f0)
```Python
import plotly.express as px
df=px.data.tips()
fig = px.pie(df, values='total_bill',names='day')
fig.show()
```

![image](https://github.com/user-attachments/assets/17498d6f-6e96-45f9-8a3f-cce7b822b51b)

# RESULT:
Thus , To implement Dashboards creation with Plotly and Dash using python is successfully done.


<h1 align="center">Data Science Tool Kit</h1>

<p align="center"><a href="https://blackbird.ai/"><img src="./image/python.png"></img></a></p>


## Description:
**Name of Event** with Description of the event and link. 

## Notes:
#### ML in Python | [SciKit](https://scikit-learn.org/stable/)
- Simple and efficient tools for predictive data analysis: Regression, Classification, Clustering, Support Vector Machines, Dimensionality Reduction
- Built on [NumPy](https://numpy.org/), [SciPy](https://scipy.org/), [pandas](https://pandas.pydata.org/) and [matplotlib](https://matplotlib.org/)
- Linear Model: 
    
    Import the relevant Libraries
    ```
    import numpy as np
    import pandas as pd
    import matplotlib.pyplot as plt
    important seaborn as sns
    sns.set()

    from sklearn.linear_model import LinearRegression
    ```
    Load the data
    ```
    data = pd.read_csv("1.01. Simple Linear Regression.cvs")
    data.head()
    ```
    Create the Regression
    ```
    x = data["col1"]
    y = data["col2"]
    x.shape
    y.shape

    x_matrix = x.values.reshape(-1, 1)
    x_matrix.shape
    ```
    Regression Itself
    ```
    reg = LinearRegression()
    reg.fit(x_matrix,y)
    ```
    R-squared
    ```
    reg.score(x_matrix, y)
    ```
    Co-efficients
    ```
    reg.coef_
    ```
    Intercept
    ```
    reg.intercept_
    ```
    Making Predictions
    ```
    reg.predict(<number>)
    ```
- [Feature Scaling](https://en.wikipedia.org/wiki/Feature_scaling) is a method used to normalize the range of independent variables or features of data
- Differences between the L1-norm and the L2-norm [Least Absolute Deviations and Least Squares](https://www.chioka.in/differences-between-the-l1-norm-and-the-l2-norm-least-absolute-deviations-and-least-squares/) 



#### AI Applications | [MCP - Model Context Protocol](https://modelcontextprotocol.io/docs/getting-started/intro)
- Generation information from the speaker here


## Resources:
- Blackbird.AI is focusing on Kursk Incursion (2024):
    - **Compass Context** to verify and contextualize the information you see [online](https://blackbird.ai/compass-context/)


## Contact:
<!--- You can add in your linkedin, medium, stack overflow, dev.to account, etc. here --->
If you want to contact me you can reach me at <nelson@oakhalo.com>.

Connect with me on <a href="https://www.linkedin.com/in/ayla-nelson/">LinkedIn</a>

Connect with me on <a href="https://github.com/oakHalo">Oakhalo.dev</a>

<!-- 
### TODO stx: 
Future Structure (stx):
backend
frontend
images
screenShots [contains video link]
troubleShooting [contains issues resolved]
-->

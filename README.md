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
    [R-squared](https://en.wikipedia.org/wiki/Coefficient_of_determination) - Coefficient of Determination
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
    Regression Model Summary from [Scikit-Learn](https://www.geeksforgeeks.org/python/how-to-get-regression-model-summary-from-scikit-learn/) INPUT:
    ```
    # import packages
    import numpy as np
    import pandas as pd
    import statsmodels.formula.api as smf

    # loading the csv file
    df = pd.read_csv('headbrain1.csv')
    print(df.head())

    # fitting the model
    df.columns = ['Head_size', 'Brain_weight']
    model = smf.ols(formula='Head_size ~ Brain_weight',
                    data=df).fit()

    # model summary
    print(model.summary())
    ```
    Regression Model Summary from [Scikit-Learn](https://www.geeksforgeeks.org/python/how-to-get-regression-model-summary-from-scikit-learn/) OUTPUT:
    <p align="center"><a href="https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html"><img src="./image/StatsModel.png"></img></a></p>
    **P > |t|** if a variable as a p-value > 0.05, we can disregard it

    Creating a Summary Table: Features, Coefficients, P-values
    ```
    reg_summary = pd.DataFrame(data = x.columns.values, columns=['Features'])
    reg_summary
    ```

    Standardization
    ```
    from sklearn.preprocessing import StandardScaler
    scaler = StandardScaler()
    scaler.fix(x)
    x_scaled = scaler.transform(x)
    ```
- [Seaborn](https://seaborn.pydata.org/generated/seaborn.displot.html) several approaches for visualizing the univariate or bivariate distribution of data, including subsets of data defined by semantic mapping and faceting across multiple subplots
```
penguins = sns.load_dataset("penguins")
sns.displot(data=penguins, x="flipper_length_mm")
```
<p align="center"><a href="https://seaborn.pydata.org/generated/seaborn.displot.html"><img src="./image/Penguin.png"></img></a></p>

- [Underfitting](https://www.ibm.com/think/topics/underfitting) the model has no captured the underlying logic of the data
- [Overfitting](https://www.ibm.com/think/topics/overfitting) Our Training has focused on the particular training set so much, it has "missed the point" 

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

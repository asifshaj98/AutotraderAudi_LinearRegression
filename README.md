# AutotraderAudi_LinearRegression
Linear Regression on Audi cars from the AutoTrader website
# EDA
### Process
* Removing the ULEZ column, as it is entirely filled with nulls
* Dropping nulls in year, fuel, mileage, body, and transmission
* Formatting rows
* Converting owners to integer

#### Heatmap
```python
sns.heatmap(data=df8.corr(),
            annot = True,
            square = True
            )
plt.show()
```
### Heatmap
![heatmap](https://user-images.githubusercontent.com/108241576/218771535-7c063b78-3fc0-41eb-b22f-e64188433a6e.png)

### Pairplot
![pairplot](https://user-images.githubusercontent.com/108241576/218772105-81af2df8-279b-4fc1-8154-8cf5cc39d7b3.png)

### Boxplot

```python
plt.figure(figsize = (20, 5))
                
sns.boxplot(data = df8['price'],
            orient = 'h')
plt.show()
     
```
![box1](https://user-images.githubusercontent.com/108241576/218772741-aed3955c-304e-44cf-b7a0-582508a9e014.png)

```python
plt.figure(figsize = (20, 5))
                
sns.boxplot(data = df8['mileage'],
            orient = 'h')
plt.show()
     
```
![box2](https://user-images.githubusercontent.com/108241576/218773838-39a668e9-bc53-4b3e-89e6-2dde3b6e4445.png)


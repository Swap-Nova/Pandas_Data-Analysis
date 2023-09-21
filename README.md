## Getting Started with Pandas:
- Pandas are used to explore data, analyze data, and manipulate data that is used in the ML field. Sometimes we have to make our raw data and manipulate it through pandas to make it in a form that ML algorithms can understand.
- There are two data types in Pandas:
  1. Series: It is a dimensional data type where we define a single object in an array manner.
```python
series = pd.Series(["BMW", "Honda", "Audi"])
# To print the output
series
```
  2. Dataframe: A two-dimensional data type that takes a Python dictionary. Moreover, it can take the data from a series as well.
- To get started
```python
car_data = pd.dataframe({"Car Make": series, "Color": colors})
# to print the output
car_data
```
<img width="683" alt="Screenshot 2023-09-22 at 12 06 03 AM" src="https://github.com/Swap-Nova/Pandas_Data-Analysis/assets/92979885/0acb1483-2abd-4a34-867e-33d3d98c339a">

## Importing Data through URLs:
- Make sure that make sure the dataset is in the "raw" format, by clicking the raw button on GitHub.
```python
heart_disease = pd.read_csv("https://raw.githubusercontent.com/mrdbourke/zero-to-mastery-ml/master/data/heart-disease.csv")
```

## Describing Data with Pandas
<table style="width:100%">
  <tr>
    <th>Attributes</th>
    <th>Functions</th>
  </tr>
  <tr>
    <td>car_sales.dtypes</td>
    <td>Meta information which is stored in car sales data frame</td>
  </tr>
  <tr>
    <td>car_sales.to_csv()</td>
    <td>Series of steps performed to execute the cmd</td>
  </tr>
</table>

## Difference between .loc and .iloc:
- .loc (location): We can manually define the location of the object inside the array and then call the object by mentioning the location assigned to it. This refers to the index.
```python
# .loc : Location
animals = pd.Series(["cat", "dog", "panda", "owl"], index=[0, 3, 9, 3])
animals.loc[3]

# OUTPUT:
3    dog
3    owl
dtype: object
```

- .iloc (integer location): In the above code we have defined the animal data series and when we call it using iloc, it will give the array object of that location. This refers to position.
```python
# .iloc refers to position 
animals.iloc[3]

# OUTPUT:
'owl'
```

## Replacing String to Int:
```python
price_plot = car_sales["Price"].replace('[\$\,\.]', '', regex=True).astype(int)
```
- Regex is a sequence of characters that defines a search pattern. In Python, regex is implemented in the re-module. Regex patterns can be used to match, search, replace, or extract specific text from a string.

## Using Matplotlib:
<img width="646" alt="Screenshot 2023-09-22 at 12 15 07 AM" src="https://github.com/Swap-Nova/Pandas_Data-Analysis/assets/92979885/5048643a-f1fb-44e6-8e67-3514514be5a4">

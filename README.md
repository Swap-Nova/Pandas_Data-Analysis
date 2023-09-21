<h2> Getting Started with Pandas </h2>
- It is a data analysis tool to explore data, analyze data, manipulate data that is used in ML field.

- There are two main data-types in Pandas:
<ol>
    <li>Series: It is one dimensional data type where we defined a single object in an array-manner. </li>
    ```python
        series = pd.Series(["BMW", "Honda", "Audi"])
        # To print the output
        series
    ```
    <li>Dataframe: It is two-dimensional data type where it takes a python dictionary. Moreover it can take the data from an series as well.</li>
    ```python
        car_data = pd.dataframe({"Car Make": series, "Color": colors})
    # to print the output
    car_data
    ```
</ol>
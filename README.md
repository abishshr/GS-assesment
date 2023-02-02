# GS-assesment

This Jupyter notebook contains a script that demonstrates the process of batch aggregation of weather data using PySpark. The weather data contains the metrics temperature and precipitation, their respective values, and the timestamp of measurement.

The script consists of the following steps:

    Input Data: Metric, Value, and Timestamp
        The weather data is stored as a list of rows, each row contains the metric, its value, and the timestamp.
        The data is then written to a CSV file input_data.csv.

    Setting Up Spark Environment for Batch Aggregation
        The necessary PySpark modules are imported and a Spark context and session are created.

    Loading the Source Data into a Dataframe
        The data is loaded from the CSV file into a PySpark dataframe.

    Data Preprocessing and Cleaning
        The data types of columns are changed to the appropriate ones.
        The timestamp column is casted as a Timestamp type.

    Batch Aggregation
        The data is aggregated by metric and the average value, max and min is computed for each metric.
        

    Saving the Results
        The aggregated data is saved to a CSV file aggregated_data.csv
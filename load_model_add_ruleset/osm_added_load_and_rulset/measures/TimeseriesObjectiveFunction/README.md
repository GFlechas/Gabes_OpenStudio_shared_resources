

###### (Automatically generated documentation)

# TimeSeries Objective Function

## Description
Creates Objective Function from Timeseries Data

## Modeler Description
Creates Objective Function from Timeseries Data.  The measure applies a Norm at each timestep between the difference of CSV metered data and SQL model data. A timeseries plot can also be created.  Possible outputs are 'cvrmse', 'nmbe', 'simdata' = sum of the simulated data, 'csvdata' = sum of metered data, 'diff' = P Norm between the metered and simulated data if Norm is 1 or 2, else its just the Difference.

## Measure Type
ReportingMeasure

## Taxonomy


## Arguments


### Path to CSV file for the metered data
Path to CSV file including file name.
**Name:** csv_name,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### CSV Time Header
CSV Time Header Value. Used to determine the timestamp column in the CSV file
**Name:** csv_time_header,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### CSV variable name
CSV variable name. Used to determine the variable column in the CSV file
**Name:** csv_var,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Convert Units
Convert Units in Metered Data
**Name:** convert_data,
**Type:** Choice,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### CSV variable display name
CSV variable display name. Not yet Implemented
**Name:** csv_var_dn,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Year in csv data timestamp
Is the Year in the csv data timestamp => mm:dd:yy or mm:dd (true/false)
**Name:** year,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Seconds in csv data timestamp
Is the Seconds in the csv data timestamp => hh:mm:ss or hh:mm (true/false)
**Name:** seconds,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### SQL key value
SQL key value for the SQL query to find the variable in the SQL file
**Name:** key_value,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### TimeSeries Name
TimeSeries Name for the SQL query to find the variable in the SQL file
**Name:** timeseries_name,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Reporting Frequency
Reporting Frequency for SQL Query
**Name:** reporting_frequency,
**Type:** Choice,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Environment Period
Environment Period for SQL query
**Name:** environment_period,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Norm of the difference of csv and sql
Norm of the difference of csv and sql. 1 is absolute value. 2 is euclidean distance. 3 is raw difference.
**Name:** norm,
**Type:** Double,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Scale factor to apply to the difference
Scale factor to apply to the difference (1 is no scale)
**Name:** scale,
**Type:** Double,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Find Available data in the SQL file
Will RegisterInfo all the 'EnvPeriod', 'ReportingFrequencies', 'VariableNames', 'KeyValues' in the SQL file.  Useful for debugging SQL issues.
**Name:** find_avail,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### algorithm_download
Make JSON data available for algorithm_download (true/false)
**Name:** algorithm_download,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### plot_flag timeseries data
Create plot of timeseries data (true/false)
**Name:** plot_flag,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Plot name
Name to include in reporting file name.
**Name:** plot_name,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### verbose_messages
verbose messages.  Useful for debugging but MAJOR Performance Hit.
**Name:** verbose_messages,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### warning_messages
Warn on missing data.
**Name:** warning_messages,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### add_first_zero_for_plots
Add a point of zero value to the plot at the beginning of the runperiod.
**Name:** add_first_zero_for_plots,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### add_last_zero_for_plots
Add a point of zero value to the plot at the end of the runperiod.
**Name:** add_last_zero_for_plots,
**Type:** Boolean,
**Units:** ,
**Required:** true,
**Model Dependent:** false





## Outputs












diff, simdata, csvdata, cvrmse, nmbe



###### (Automatically generated documentation)

# Timeseries Plot

## Description
Creates an interactive timeseries plot of selected variable.

## Modeler Description
NOTE: This will load and respond slowly in the OS app, especially if you select * on a variable with many possible keys or you select timestep data.  Suggest you open it in a web browser like Chrome instead.

## Measure Type
ReportingMeasure

## Taxonomy


## Arguments


### Enter Variable Name.
Valid values can be found in the eplusout.rdd file after a simulation is run.
**Name:** variable_name,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Reporting Frequency.

**Name:** reporting_frequency,
**Type:** Choice,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### Enter Key Name.
Enter * for all objects or the full name of a specific object to.
**Name:** key_value,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false

### availableEnvPeriods
availableEnvPeriods
**Name:** env,
**Type:** String,
**Units:** ,
**Required:** true,
**Model Dependent:** false





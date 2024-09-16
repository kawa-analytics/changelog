# Changelog: Version 1.26 (Sept. 10th 2024)


## New features

- __Editable datasources__: Introduce the ability to edit datasources directly in the GUI with a UI similar to Excel or Google sheet.

- __Python datasources__: Add a new datasource type that is connected to a python script. The execution of the script can be scheduled to feed the data.

- __Github and Gitlab integrations__: New connection between KAWA and source control systems to load python scripts directly into the application. Those scripts can be used for Automations, Python datasources (see above) and Python columns.

- __Map chart__: Added a new chart type to plot metrics per country on a map.

- __Filters__: Added new options for text filters. The users can now group values into categories and filter based on those categories.

- __Event Log__: Added a scheduled job to apply a retention policies on the event table. This will keep its size to a reasonable upper limit.


## Improvements

- __Dashboards__: Improved the UX and UI of dashbaord filters

- __Python library - download speed__: Speed up computations made from the python library. Computations that require the transfer of big datasets between KAWA and the Python runtime can benefit from a x3 speedup.

- __Python library - support of arrow streaming for uploads__: A new method is now available from the kawa client which lets the client code send data directly in the arrow streaming format to Clickhouse. This is quicker than the previous method that require the seriazlisation of the dataframes into parquet files.

```python
 loader = self.kawa.new_arrow_data_loader(
            arrow_table=arrow_table,
            datasource_name='Sample'
        )
```


## Bug fixes

- Handle visibility for columns in expression editor and add fields section
- Script preview is broken when editing an automation
- Dashboard - error when opening "apply to" settings for filter in case if one of the target sheets was removed
- Problem with display of dashboard refresh rate
- Box plot shows wrong min
- Formula generator gets parenthesis wrong
- Bug when factorizing SQL queries (FActoring has been enabled following the fix for this bug)
- Issue when switching datasources quickly
- Formatters - overflow for dropdown


# Changelog: Version 1.28 (Dec. 16th 2024)

## New features

__Applications__:

A new section was added to KAWA: Applications.
They let users create rich web applications that can be published.
In version 1.28, applications can contain Views and Dashboards as pages.
Each page can be configured to restrict the interactions that consumers of
the applications will be able to do (Filtering, Sorting, Grouping, Deploying/Folding nodes etc)

If AI is configured, applications also feature a dedicated assistant to interact with the data in scope with natural language.


__Python script parameters__:

Python scripts now have parameters in addition to inputs, outputs and secrets. These parameters will be set when users define Buttons in Control panels.

__Chat with your data (beta)__:

A brand new AI chat is included in the Application section.
It brings the capabilities to query all the sheets in the application scope,
as well as the ability to manage multiple user uploaded files.


## Improvements


- KAWA will now write date and datetime objects in clickhouse instead of timestamps

- Support for HTTP header based Authentication (SSO)

- Improve workspace management mechanism

- Remove the need to share objects (Sheets, columns) when using them in Dashboards and Applications

- Simplify the Workspace flags

- Allow to re synch live connected data source to update the schema

- Python: Allow append only ingestions


## Bug fixes


- Dashboard - errors on dashboard change if edit widget mode was enabled
- Dashboard - column name is n/a for cross filter
- Add filter in dashboard app edit mode doesn't work
- When sharing a dashboard, the layout is broken
- Glitch when searching for a column in the model
- Glitch when setting attribute
- Dashboard - shield is not working for cross filtering
- Chart - find and fix problems caused to allow to use more the 2 levels of groups
- Block source control change
- Fix the use of Date and DateTime indexes
- Issue with connection to Flight Server
- Gitlab does not refresh after commit
- Should not be able to create python column on external tables without primary keys
- Dashboard - clear auto refresh interval on component destroy
- Control: exception raised when adding multi-select control using the values of existing column



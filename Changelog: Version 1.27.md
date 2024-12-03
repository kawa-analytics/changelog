# Changelog: Version 1.27 (Nov. 1st 2024)

## New features

__Enhanced Sharing mechanism__:

We’re excited to introduce enhanced sharing capabilities, giving you more control over who can access and edit shared objects, such as Dashboards, Datasources, and Sheets within your workspace. 

You can now share objects with specific teams and assign either **VIEW ONLY** or **EDIT** access to each team.

Additionally, you can define general access for all other members of the workspace:

1. **RESTRICTED:** Only specified teams can access.
2. **VIEWER:** Anyone in the workspace can view the object.
3. **EDITOR:** Anyone in the workspace can edit the object.

__New AI Co-Builder Feature (beta)__:

We’re excited to introduce KAWA’s AI Co-Builder, a new feature designed to help you rapidly create custom data applications. 


## Improvements


- Fix of date/datetime handling with ClickHouse

- Ability to connect to tables in other ClickHouse databases

## Bug fixes

- Handle visibility for columns in expression editor and add fields section
- Script preview is broken
- Number filter: Apply button is disabled when "Condition" tab is selected and value is "0" -> impossible to apply filter
- Shared dashboard issues
- Issue with sorting cycle
- Indicator charts are broken
- Issue when switching datasources quickly
- Application version is no longer showing up
- Formatters - overflow for dropdown
- Publish button is missing on views


## Patches

### Version 1.27.1 (November 22nd 2024)

- Fix pivot first column width
- Fix selection in Control panel multi select
- Fix formula edition when parameters are involved
- Add signup feature flag


### Version 1.27.2 (December 4th 2024)

- Fix support for `<=` and `<` in formula editor
- Fix date and date time indexes
- Allow to use both integers and decimals in IF branches
- Fix Rendering of number formats (Red color)




# Changelog: Version 1.29 (Feb. 14th 2024)

## New features

__Knowledge__:

A new section was added to KAWA: Knowledge.
This section lets user connect their unstructured data with KAWA.
It requires a connection between KAWA and an OCR and and completion API. 


__Data Preparation v1__:

KAWA has an improved data subsection in the datasource section.
It gives insights and stats about the dataset, globally and per column.
It also lets users perform sumple transformations their data directly from the datasource section.

__Window functions__:

KAWA now supports WINDOW functions directly from the formula editor.
You can now directly use formulas such as: Sliding average, cumulative sums etc...

__Dry run mode__:

You now have the options to disable automatic computations on all the views. This is particularly useful when you are working on a computating intensive view and that you want to apply groups of changes before generating the final result.



## Improvements


- Improve UX to create data enrichments in sheets. A single button will now expose: formulas, mappings, python columns, lookup columns.



## Bug fixes


- Impossible to show chart when sheet is shared with teams
- Formula editor context switch loses the formula
- Nested call expressions do not work
- ABS DESC/ASC not available in pivot
- Script - share dialog is broken
- Expression-editor - error with AI formula generation
- Problem When adding lookup columns and picking multiple columns to add
- Cannot insert tokens in the first position
- Formula editor - Clear error message as soon as generation works
- Bug when using Blockly and new dep system
- When a Python ETL fails, the error status does not propagate to the sheet
- Chart - resize issue
- In linked column, make configuration viewable even if not editable
- Automations - hide action buttons in CP


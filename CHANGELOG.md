# Redocly OpenAPI VS Code Extension

## Release 0.1.0 (2021-11-18)

### Features

- The extension now supports **interactive controls** for `info`, `server`, and `externalDocs` sections. To activate interactive controls, open the cursor context panel and place the cursor into any of the supported sections. The cursor context panel will show the visual OpenAPI editor where you can modify the contents of the supported sections directly. Your changes are immediately reflected in the API definition file.

- You can now use the `htmlTemplate` option in your `.redocly.yaml` configuration file to style the look of the live documentation preview.

- The live preview panel now automatically scrolls to the section of the API definition you're editing. More specifically, the following behavior has been implemented:

  - Editing a tag scrolls to the tag section
  - Editing a path item scrolls to the first operation in the path item
  - Editing an operation scrolls to the operation
  - Editing a schema scrolls to the first operation that uses the schema

### Fixes

- Implemented a number of performance and stability improvements.
- The autocompletion feature now automatically switches to a new line if the selected item is not a scalar type. It also makes it easier to move to a new line on the same level as the current item by providing the `newLine` option in the suggestion dropdown.
- Improved the suggestions for the `referenceDocs` section of the `.redocly.yaml` configuration file.
- Root-level items in the suggestion dropdown are now sorted according to the OpenAPI specification. 

----

## Release 0.0.15 (2021-10-21)

### Features

- Fields in YAML files that contain a link to an internal file now support the *Go to...* option. Use this option to quickly access files in your project - for example, to open referenced API definitions directly from the `apiDefinitions` section in `.redocly.yaml`.

- Improved autocompletion and validation for the `.redocly.yaml` configuration file.

### Fixes

- Improved the performance of the documentation preview on first load.

- Internal improvements to YAML parsing.

----

## Release 0.0.14 (2021-09-16)

### Features

- The extension now supports a new panel: the cursor context, where you can learn more about OpenAPI objects and properties you're editing. Select the *Open cursor context* icon in the VS Code toolbar to open the panel. The descriptions in the panel are context-aware, and will change as you place your cursor into different sections of your OpenAPI document. 

- The live documentation preview feature now requires an API key from Redocly. When you open the *Preview* panel, you will find the instructions for how to obtain the key.

- Improved the performance of validation and autocompletion in all types of files, including OpenAPI documents, referenced files (linked with $ref in OpenAPI documents), and configuration files.

- Renamed the *Reference Docs* panel to *Preview*.

----

## Release 0.0.13 (2021-09-02)

### Features

- Implemented autocompletion for configuration files. When editing the `referenceDocs` section of the `.redocly.yaml` file, you will now get a list of all supported configuration options in the suggestions widget.

----

## Release 0.0.12 (2021-09-01)

### Features

- Implemented validation of the `.redocly.yaml` file.
- Improved autocompletion for media types.

----

## Release 0.0.11 (2021-08-30)

### Fixes

- Changed the storage location of images in the README.

----

## Release 0.0.10 (2021-08-27)

### Features

- The preview panel now uses the styling from the VS Code theme.
- The live preview now updates and saves state even when running in the background (when the preview panel is closed).

----

## Release 0.0.9 (2021-08-23)

### Features

- Editing `apiDefinitions` in `.redocly.yaml` updates the definition list in the Reference docs preview panel.

----

## Release 0.0.8 (2021-08-18)

### Features

- The preview panel now uses Reference docs instead of Redoc to generate the documentation preview.
- The preview panel uses settings from the `.redocly.yaml` file.
- Implemented preview persistence (restores the view state after going to background and between VS Code restarts).
- The active definition button is highlighted in the preview.
- Names from the `apiDefinitions` list are now used in the preview instead of file names.

### Fixes

- Fixed default validation rules for non-existing `.redocly.yaml` file (which resulted in errors not being reported).

### Known issues

- The `.redocly.yaml` file must be saved to disk (Ctrl+S) for changes to apply.

----

## Release 0.0.7 (2021-08-16)

### Features

- The `.redocly.yaml` initialization prompt is not shown anymore if the user previously declined initialization for that workspace.
- Updated the README and renamed openapi-vs-code to Redocly OpenAPI in it.

----

## Release 0.0.6 (2021-08-16)

### Features

- Added a prompt for the `.redocly.yaml` file initialization.
- Renamed the extension from openapi-vs-code to Redocly OpenAPI in the Marketplace.

### Fixes

- Fixed linting exceptions.

----

## Release 0.0.5 (2021-08-13)

**First public release!** 🥳

### Features

- Continuous OpenAPI linting
- OpenAPI completion
- Go-to-definition for OpenAPI $refs
- Built-in API documentation preview powered by Redoc

----

## Releases 0.0.4 - 0.0.1

Internal development releases.


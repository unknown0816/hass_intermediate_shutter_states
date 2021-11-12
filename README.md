# Home Assistant intermediate shutter states

## Introduction

This is a small example how to add custom icons to Home Assistant and use them for intermediate states. Home Assistant just uses the states 'open', 'opening', 'closing' and 'closed'.
To extend this with intermediate states if conditions checking the current position of the shutter were added to the configuration.yaml. This is using [custom-ui](https://github.com/Mariusthvdb/custom-ui) for Home Assistant.
Further, 3 new icons were added to Home Assistant to provide each state with an icon. The icons are added using the custom_icons.js file.
However, they can be viewed in the repository as svg-files.

## Installation

* [Install custom-ui](https://github.com/Mariusthvdb/custom-ui/blob/master/INSTALLING.md)
* Copy the js-file into your local resource directory of Home Assistant (in my case the 'www'-directory) and add the file via Lovelace resource or via configuration.yaml
```yaml
frontend:
  extra_module_url:
     - /local/custom_icons.js
```
* Add the content of the configuration.yaml to your configuration.yaml

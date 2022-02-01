# Discord DM message tool

Reads discord text channel logs and makes data tables from them  
presumably all versions are a bit broken so just clone from master and hope

## Dependencies
All depend on [Discord Chat Exporter](https://github.com/Tyrrrz/DiscordChatExporter) and getting the logs from there.
Install and  run the program, for your user token [they have a guide](https://github.com/Tyrrrz/DiscordChatExporter/wiki/Obtaining-Token-and-Channel-IDs)

Python specific dependencies:
 ```pandas, python-dateutil, plotly```

And then a bunch of imports that should be in the base python libs

## Getting the logs
For safety before download click on the cog and for time format setting input ```u```
In discord chat exporter, navigate the GUI to download the channels you whish.
When prompted for a format, select JSON and then save to a folder without any .json files. You will be asked to provide a path to this folder later.

## Running 
If you want a graph you'll want to run graph.py
If you want to get the pandas dataframe import table.py and run main which returns a dataframe

## Config
If a config file is not present, the program will prompt user for parameters which are then saved
WARNING : right now there's no support for multiple config files. If at least one file is found the first one will be used
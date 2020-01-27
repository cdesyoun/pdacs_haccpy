# PDACS HACC Data portal browser
HACC data portal as galaxy data resource is configured as galaxy tool.
This is an example for the interaction of Galaxy with an external data source.

## Galaxy configuration
In Galaxy, the external data source is implemented as a tool with a specific type, "data_source".
You need to configure the "[galaxy/config/tool_conf.xml.sample](galaxy/config/tool_conf.xml.sample)", and copy the "[galaxy/tools/data_source/pdacs_hacc.xml](galaxy/tools/data_source/pdacs_hacc.xml)" into the Galaxy.

## CherryPy server
As the external source, CherryPy, which is a python module for a minimalistic web server, was chosen. 
CherryPy takes away some of the work which would be needed starting from SimpleHTTPServer.
### The deployment process is as follows:
```shell
% virtualenv -p python3 venv_haccpy
% source venv_haccpy/bin/activate
% pip install cherrypy
% python server.py
```

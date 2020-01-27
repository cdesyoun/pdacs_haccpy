# PDACS HACC Data portal browser
HACC data portal as galaxy dataresources is configured as galaxy tool.

## galaxy configuration
This is an example for the interaction of Galaxy with an external data source, that is hacc data portal.
```shell
% virtualenv -p python3 venv_haccpy
% source venv_haccpy/bin/activate
% pip install cherrypy
% python server.py
```

# Portable Node-RED

Run Node-RED with local settings.  
Node-RED with default options stores settings file to user directory like ``%USERPROFILE%\.node-red``.  
This configured repository has options to store settings in local directory.  


## Prepare

```sh
git clone git@github.com:ryoichi-obara/node-red-run-local.git
cd node-red-run-local
npm i
```

## Run

```sh
npm start
```


## Portable settings

``package.json`` in this repo uses ``--userDir`` and ``--flowFile`` options to run Node-RED.
The options specify location to store in your local directory.


## Debug in VS Code

For debugging purpose, this repository has ``./vscode/launch.json``.  
You can debug your code / your Node-RED execution easily in VS Code.  

launch.json has two options to debug.
Both are useful for your debugging.
One is to run Node-RED in VS Code debugging feature.  
The other one is to pick up process that have already running.  

### Debug to run Node-RED

* Click debug pane on side menu.
* Select a configuration "Run Node-RED".
* Start debugging

### Debug to pick process

* Run Node-RED e.g. ``npm start``
* Click debug pane on side menu.
* Select a configuration "Pick process".
* Start debugging

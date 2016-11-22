# REALZ

An experiment in combining Node, React, and A-Frame

REALZ:

• React, Redux, RethinkDB

• A-Frame (http://aframe.io)

• Horizon (Node) (http://horizon.io)

## Installation

  - Install Horizon: http://horizon.io/install/
    (this will include installing RethinkDB)

  - Download the REALZ source code
  - cd into REALZ directory
  - hz serve --dev
  - Open http://127.0.0.1:8181

## Restarting

When stopping the Horizon server, kill with control-Z (not control-C). When restarting, Horizon server, an error can occur:

    HTTP server: Error: listen EADDRINUSE 127.0.0.1:8181

To fix, first do this to show running processes:

    lsof -i tcp:8181

Then this, where [PID#] is the process PID (example, 8875):

    kill -9 [PID#]

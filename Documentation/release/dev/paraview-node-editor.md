## ParaView Node Editor

Integration of the project https://github.com/JonasLukasczyk/paraview-node-editor

### Overview

This plugin contains a node editor for ParaView that makes it possible to conveniently modify filter/view properties, filter input/output connections, as well as the visibility of outputs in views.
The editor is completely compatible with the existing ParaView widgets such as the pipeline browser and the properties panel (one can use them simultaneously).

### User Manual

* Filters label :
    - Left click : select filter as active source
    - Left click + CTRL : add filter to the current selection
    - Middle click : Delete the filter
    - Right click : toggle between invisible, normal and invisible mode for the filter properties
* Filters input ports :
    - Left click + CTRL : set all selected output ports as input. If only one input is accepted it will use the last selected object as input.
    - Middle click : Clear all incoming connections for this port
* Filters output ports :
    - Left click: set output port as active selection
    - Left click + CTRL: add output port to current selection
    - Left click + SHIFT: toggle visibility in active view
    - Left click + SHIFT + CTRL: hide all but this port in active view
* View label :
    - Left click : select as active view
    - Right click : increment verbosity
* Drag and drop from a port to an other to create links between 2 filters. This is not supported between a view node and a filter yet.

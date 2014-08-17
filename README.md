###trRefsUpdater
Copyright 2014, Triada Studio

by Vahan Sosoyan sosoyan@gmail.com

===

This module helps to iterate through all referenced files in the current maya scene, check for updates and replace with the new versions.

![](https://dl.dropboxusercontent.com/u/11663164/shared/trRefsUpdater_Demo.gif)

===

###Installation

Just clone trRefsUpdater.py and userSetup.py to your maya scripts directory, or if you already have userSetup.py, then add this lines above.

```bash
import maya.utils as utils
import trRefsUpdater

utils.executeDeferred('trRefsUpdater.refsUpdaterCallback()')
```

###Usage

As soon, as you open Maya scene, the callback script will automatically check for new filename versions of all  reference objects in the scene and in case there are any in place, will offer to update them.

Also can be used as seperate command.

```bash
import trRefsUpdater

trRefsUpdater.refsUpdater()
```
Custom `il` ( if loaded ) and `tr` ( top reference ) flags are available to make it fit in your pipeline.

```bash
refsUpdater([il=boolean],[tr=boolean])
```

**NOTE:** by default both flags are True.

###trRefsUpdater

###Installation

Clone this repo into your maya scripts directory, or if you already have userSetup.py, then add this lines above.

```bash
import maya.utils as utils
import trRefsUpdater

utils.executeDeferred('trRefsUpdater.refsUpdaterCallback()')
```

###Usage

As soon, as you open Maya scene, the callback script will automatically check for new filename versions for all  reference objects in the scene and in case there are any in place, will offer to update them.

Also can be used as seperate command.

```bash
import trRefsUpdater

trRefsUpdater.refsUpdater()
```

License
-------
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

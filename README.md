fmbt-tizentest
================

This example demonstrates generating and running tests against the
File Manager sample application on Tizen 2.3.


Prerequisites
-------------

- Install fMBT, version 0.9 or later is required.

- Install Tizen SDK 2.3.

- Configure and launch Tizen device emulator

- [Install](https://github.com/amazpyel/fmbt-tizentest/blob/master/python_install.md) libpython-2.7.1-1.4.i586.rpm and python-base-2.7.1-1.4.i586.rpm on emulator 

- [Build and install](https://github.com/amazpyel/fmbt-tizentest/blob/master/filemanager_installing.md) File Manager Sample application on emulator.

- If everything is ok, you can open Tizen device screenlock by executing:

$  python -c 'import fmbttizen; fmbttizen.Device().swipe((0.1, 0.8), "east")'


Running a test
--------------

- Navigate to the homescreen on Tizen device.

- Launch the test:

$ fmbt smoke.conf


Debugging a test
----------------

d.enableVisualLog(...) in filemanager.aal starts logging whatever happens in
the Device instance. The log is written to devicelog.html. Open the
log with your browser:

$ chromium devicelog.html


Model & adapter design
----------------------

See the model & adapter:

$ fmbt-editor filemanager.aal

filemanager.aal enables testing

- activating File Manager application.

- creating folder

- deleting folder 

fMBT official repo
-----------------------
https://github.com/01org/fMBT

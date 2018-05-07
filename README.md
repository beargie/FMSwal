# FMSwal
FileMaker Implementation of SweetAlert (http://sweetalert.js.org/). Modular file spawns alerts using card windows and dynamic layouts.

## Installation Instructions
* Easiest way is to host the fmswal.fmp12 file along with any file you want to use it with. 

* Use a "perform script" script step to perform the "fmswal" script from the fmswal.fmp12 file. 

* See the "complete demo" script for an example of the formed JSON parameters in order to pass parameters for styling alerts.

* Utilize Get(ScriptResult) in your own script to handle the result from the alert.

## Important Considerations
* Due to WebDirect's lack of card window support, this package is not recommended for WebDirect.
* SECURITY! Files are provided unlocked with the default username and password as of FM16. Please make sure to set your own password and appropriate security for deployment! Here are some quick thoughts on securing it
  * Change the admin account name to a different account name.
  * Add a password for the Full Access account
  * Add a restricted privelege set that has no access to layout mode, editing scripts, creating or deleting records, remove the ability to change passwords or error dialogs.
  * Add a new user with the restricted privilege set.
  * Set File > File Options to auto-login with the restricted user.
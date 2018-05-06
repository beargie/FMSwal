## FMSwal
FileMaker Implementation of SweetAlert (http://sweetalert.js.org/). Modular file spawns alerts using card windows and dynamic layouts.

# Installation Instructions
* Easiest way is to host the fmswal.fmp12 file along with any file you want to use it with. 

* Use a "perform script" script step to perform the "fmswal" script from the fmswal.fmp12 file. 

* See the "complete demo" script for an example of the formed JSON parameters in order to pass parameters for styling alerts.

* Utilize Get(ScriptResult) in your own script to handle the result from the alert.

# Important Considerations
* Due to WebDirect's lack of card window support, this package is not recommended for WebDirect.
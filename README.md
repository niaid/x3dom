README.txt
==========

ABOUT X3DOM
-----------
X3DOM is an open-source framework and runtime for web 3d graphics.
Pronounced "X-Freedom".

It supports the ISO standard X3D (Extensible 3D) file format. 

Read more at http://www.x3dom.org and http://www.web3d.org.


THE X3DOM MODULE
----------------
This module enables interaction with 3D content within Drupal
by providing an "X3D Interactive Viewer" custom display format
using the X3DOM API.

The X3DOM module depends on the Field and File modules.

For a full description of the module, visit the project page
http://drupal.org/project/x3dom.

To submit bug reports and feature suggestions, or to track changes
please use http://drupal.org/project/issues/x3dom.


INSTALLATION
------------
Install as you would normally install a contributed Drupal module.  
https://drupal.org/documentation/install/modules-themes/modules-7

Download and enable the module dependency Libraries API
http://drupal.org/project/libraries

X3DOM releases can be found at the "Get It" page on X3DOM.org
http://www.x3dom.org/?page_id=7.

Save the x3dom-full.js & x3dom.css files
to the sites/all/libraries/x3dom folder.
 - sites/all/libraries/x3dom/x3dom-full.js
 - sites/all/libraries/x3dom/x3dom.css


CONFIGURATION
-------------
The X3D Interactive Viewer format is used two ways:
 - From a Content Type's Manage Display tab for a File Field
 - Select the X3D Interactive Viewer format.  
 - Set the viewer's Width and Height in the field's Settings option.
 
 - From a View's Fields section, select a File Field type.
 - Set the field's Formatter to X3D Interactive Viewer.
 - Set the field's Width and Height.


REQUIREMENTS
------------
X3DOM runs in Javascript- and WebGL-enabled browsers.

For Safari Client Browsers
Select "Enable WebGL" in Safari's Develop menu. 
 - The Develop menu can be toggled on or off
 - In the "Advanced" tab under File > Preferences.


RECOMMENDED MODULE
------------------
It is recommended to also install the Views module
https://drupal.org/project/views
 - When enabled, users can list and sort 3D content.


KNOWN ISSUE & FIX
-----------------
There is a known issue with the current release of x3dom-full.js
 - See https://github.com/x3dom/x3dom/issues/479
 - <x3d> tag reloads do not clear lighting
 - This results in "extra lights"
 - Each JavaScript reload increases model brightness.

This issue is fixed in the "Current Dev Release" of x3dom-full.js
 - http://x3dom.org/download/dev/x3dom-full.js.
 - To apply this change to the X3DOM module:
 - Replace the x3dom-full.js file with the Current Dev Release version.
 - sites/all/libraries/x3dom/x3dom-full.js


OTHER RESOURCES
---------------
X3DOM's Issue Tracker is on GitHub at https://github.com/x3dom/x3dom.

Mailing lists for technical questions related to X3DOM are as follows:
 - User Support
 - https://lists.sourceforge.net/lists/listinfo/x3dom-users
 - Developer Support
 - https://lists.sourceforge.net/lists/listinfo/x3dom-developers


MAINTAINERS & SPONSOR
---------------------
Current maintainers of X3DOM module:
 - Makazi Mtingwa (MakaziMtingwa) - http://www.drupal.org/user/2995707
 - Nick Weber (webermn) - http://drupal.org/user/2791697

This project has been sponsored by 
the Office of Cyber Infrastructure and Computational Biology (OCICB) 
at the National Institute of Allergy and Infectious Diseases (NIAID).

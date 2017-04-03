README.txt
==========

ABOUT X3DOM
-----------
X3DOM (pronounced "X-Freedom") is an open-source framework and runtime for 3D graphics on the Web. 

It supports the ISO standard X3D (Extensible 3D) file format. 

Read more at http://www.x3dom.org and http://www.web3d.org.


THE X3DOM MODULE
----------------
The X3DOM module enables you to display and interact with 3D content within Drupal. 
Specifically, it uses the X3DOM API and provides an "X3D Interactive Viewer" custom display format.

The X3DOM module depends on the Field and File modules.

For a full description of the module, visit the project page at http://drupal.org/project/x3dom.

To submit bug reports and feature suggestions, or to track changes, please use http://drupal.org/project/issues/x3dom.


INSTALLATION
------------
Install as you would normally install a contributed Drupal module.  

See https://drupal.org/documentation/install/modules-themes/modules-7 for further information.

Download and enable the module dependency Libraries API, please use http://drupal.org/project/libraries

Save the x3dom-full.js & x3dom.css files to the sites/all/libraries/x3dom folder.
 - sites/all/libraries/x3dom/x3dom-full.js
 - sites/all/libraries/x3dom/x3dom.css


CONFIGURATION
-------------
The X3D Interactive Viewer format is used two ways:
 - From a Content Type's Manage Display tab for a File Field, select the X3D Interactive Viewer format.  
 - Set the viewer's Width and Height using the field's Settings option.
 
 - From a View's Fields section, select a File Field type.
 - Set the field's Formatter to X3D Interactive Viewer.
 - Set the field's Width and Height.


REQUIREMENTS
------------
X3DOM runs in Javascript- and WebGL-enabled browsers.

For Safari Client Browsers, select "Enable WebGL" in Safari's Develop menu. 
 - The Develop menu can be toggled on or off in the "Advanced" tab under File > Preferences.


RECOMMENDED MODULE
------------------
It is recommended to also install the Views module (https://drupal.org/project/views).
 - When enabled, users can list and sort 3D content.


KNOWN ISSUE & FIX
-----------------
This module is packaged with X3DOM's current release version of x3dom-full.js. 

X3DOM releases can be found under the "Latest Stable Release" section at http://www.x3dom.org/?page_id=7.

There is a known issue with the current release version of x3dom-full.js
 - See https://github.com/x3dom/x3dom/issues/479
 - <x3d> tag reloads do not clear lighting, resulting in "extra lights"
 - The appearance of greater brightness for each JavaScript reload.

This issue is fixed in the "Current Dev Release" version of x3dom-full.js
 - http://x3dom.org/download/dev/x3dom-full.js.
 - To apply this change to the X3DOM module, replace the x3dom-full.js file with the Current Dev Release version.
 - sites/all/libraries/x3dom/x3dom-full.js


OTHER RESOURCES
---------------
X3DOM's Issue Tracker is on GitHub at https://github.com/x3dom/x3dom.

Mailing lists for technical questions related to X3DOM are as follows:
 - User Support: https://lists.sourceforge.net/lists/listinfo/x3dom-users
 - Developer Support: https://lists.sourceforge.net/lists/listinfo/x3dom-developers


MAINTAINERS & SPONSOR
---------------------
Current maintainers of X3DOM module:
 - Meghan McCarthy 
Past contributors:
 - Makazi Mtingwa (MakaziMtingwa) - http://www.drupal.org/user/2995707
 - Nick Weber (webermn) - http://drupal.org/user/2791697

This project has been sponsored by the Office of Cyber Infrastructure and Computational Biology (OCICB) at the National Institute of Allergy and Infectious Diseases (NIAID).

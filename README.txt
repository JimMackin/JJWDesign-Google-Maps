JJWDesign Google Maps for SugarCRM

Project hosted on SugarForge.org
Do not Download ZIP from Github.com
Download ZIP from SugarForge.org
http://www.sugarforge.org/frs/?group_id=901

Created by Jeffrey J. Walters
http://www.jjwdesign.com/
Copyright (C) 2010-2014 Jeffrey J. Walters





Version 2.1.19 Changes 01/29/2014

Improvements:

1.) Revising List View Map Buttons to be built thru buildMyMenuItem() method
2.) Target new window/tab for Google directions
3.) InfoWindows: Adding basic Google Maps View link for address


Version 2.1.18 Changes 01/06/2014

Improvements:

1.) Bug: URL length issue with Google Maps libraries - moving 'current_post' into session.
2.) Bugs with SugarOnDemand: Export query where/join issues.
3.) Advanced Search link/relate field type issues.


Version 2.1.17 Changes 01/01/2014

Improvements:

1.) Adding Language File Labels
2.) Target List Map Bug: Restrict WHERE to related type and $list_id
3.) Advanced Search - Related Field Bug: Get relate/link patched 'where' and 'join'


Version 2.1.16 Changes 12/30/2013

Improvements:

1.) Marker Selection Shapes: Rectangle, Circle, Polygon
2.) Add to Target List from DataTables Listing
3.) Added Additional ACL Control Logic
4.) Various Bug Fixes and Updating Code


Version 2.1.15 Changes 12/17/2013

Improvements:

1.) Map Areas Enhancements: List Selection by Area
2.) Bug: DataTables language to lowercase
3.) Adding DataTables language en_uk.lang.js


Version 2.1.14 Changes 12/14/2013

Improvements:

1.) Bug: oDataTable reference issue
2.) Bug: Make Clusterer Images - Protocol Independent
3.) Changing links to relative URI paths
4.) Bug: Limit URI query string parameters. Used to avoid URL length errors.
5.) Bug: SugarOnDemand does not permit reading .txt files


Version 2.1.12 Changes 12/12/2013

Improvements:

1.) Point in Areas/Polygon Bug - Closing the Last Point


Version 2.1.11 Changes 12/10/2013

Improvements:

1.) Detail View map embedding issues corrected
2.) Set Geocoding API URL format check corrected
3.) Configuration settings to remove Adsense Ads
4.) JavaScript code rewriting/updating


Version 2.1.10 Changes 11/25/2013

Improvements:

1.) Click DataTables Row Marker Image to panTo Map Marker InfoWindow
2.) Corrected DataTable ID/image visibility issues
3.) Corrected Map/DataTables load/initialize issues


Version 2.1.9 Changes 11/22/2013

Improvements:

1.) DataTables TableTools Plugin referenced from CDNJS
2.) Listing Exports: Copy, CSV, Excel, PDF, Print
3.) 'Approximate' result type based on Geocoding 'location_type'
4.) Configuration setting to Allow 'Approximate' location types
5.) Debugging details for older IE browsers
6.) Code Rewriting ($bean style)


Version 2.1.8 Changes 11/20/2013

Improvements:

1.) Added Legend Marker Group Toggling
2.) Areas Module: Calculations for Area and Centroid
3.) Code Cleanup/Refactor
4.) Adding Legend Visibility to DataTables Filtering
5.) $GLOBALS Corrections
6.) Areas and Markers Modules: Map Detail/Edit Size Adjustments
7.) IFrame Auto-Height jQuery Plugin
8.) Map Target Lists by ID
9.) Geocoding 'location_type' Adjustments


Version 2.1.7 Changes 11/07/2013

Improvements:

1.) Configuration: Gecoding API URL and Support for Proxy Script
2.) Popupdef Link Correction
3.) Added DataTables Listing with Sort, Filter and Page Functionality
4.) View/IFrame URL Update
5.) Updating Logic Hooks: TODO Static Methods
6.) Improved Legend Display now as Maps Overlay
7.) Upgraded Clustering to use MarkerClustererPlus
8.) Added Map Clusterer Control Toggle
9.) Improved Language Support for Datatables
10.) Group by Field now supports enum types with DOM
11.) Corrected .json SugarOnDemand Package Scanner Issues


Version 2.1.3 Changes 10/11/2013

Improvements:

1.) Language Added for Administration Links
2.) Added logic support for "Accounts_Members" display type
3.) Map Areas: Right Click to Remove Vertex
4.) Corrected Maps Center Point Bugs
5.) Added Max Zoom Restriction to Maps
6.) Improved Throttle Control of Google Maps API Requests
7.) Map Markers: Corrected Marker Locale Bug - Edit View


Version 2.1 Changes 10/02/2013

The Map Areas module now uses the Google Maps Javascript API v3 Drawing Library to provide enhanced area editing capabilities. Several Javascript bug fixes have been included in this revision. Language files have been improved and updated for all modules.

Version 2.0.7 Changes 08/22/2013

I'm happy to announce that the JJWDesign Google Maps Package v2.0.7 now installs effortlessly on SugarCRM On-Demand. The project package now passes the Package Scanner and File Scanner requirements to allow it to install on SugarCRM On-Demand. You no longer need the assistance of SugarCRM Support to install this package, yet you will still need SugarCRM Support assistance to uninstall older versions of this package.

Version 2.0.1 Changes 02/03/2013

Serveral bug fixes have been included in this revision.


Version 2.0 Changes: 08/21/2012

Version 2.0 is a significant achievement for this project. We've come a long way from the simple idea of mapping leads. Thank you to all those who have contributed and/or donated.

Requirements:
1.) Version 2.0 now requires cURL to be installed on the server. file_get_contents() is no longer used, per SugarCRM On-Demand restrictions.

Improvements:

1.) Add Configuration Page: You can now adjust/save the majority of the settings thru this easy to use configuration form.
2.) Complete rewrite of view.map_markers.php to reduce the overall amount of JavaScript code. This was a much needed improvement. The intent is to allow the page to load faster and to be able to display a larger set of markers without crashing Internet Browsers. It should also make extending Javascript/Jquery/Google Maps API functionality much easier for future plugin development.
3.) Added functionality for mapping Meetings from the Meetings Module. Geocoding of the Meeting objects is based on the Related module type and record (flex relate). Custom list view changes.
4.) Added functionality for mapping Prospects/Targets from the Prospects Module. Custom list view changes. More on this soon.
5.) Complete rewrite of all Logic Hooks to better manage the address relationships on change (save). Several new logic hooks added. See custom/module directory for more details. This was a major overhaul of the logic hooks.
6.) Edit/Display View: Redefined the Parent Type list (flex relate field) for all Maps added in the jjwg_Maps Module. It now only allows you to select from Modules that have address information.
7.) Cache Improved: Additional logic now added to take full advantage of the Address Cache module. All successfully geocoded addresses are now stored in the Address Cache module for later retrieval.
8.) Serveral dozen or two small improvements that I don't recall at this time.
9.) Updated jQuery to version 1.8.0


Changes Specifically for SugarCRM On-Demand Users

1.) Removed instances of is_dir()
2.) Removed instanced of is_file()
3.) Removed any not acceptable file types
4.) Changed Google API Request from file_get_contents() to use PHP cURL.


Bugs:

1.) Bug: Many PHP notice messages corrected, for those running with them on.
2.) Bug: Corrected IE6 javascript error issues in view.map_markers.php
3.) Bug: CSS link path issue corrected.
4.) Bug: Corrected several bugs related to Map Areas/Markers display issues.



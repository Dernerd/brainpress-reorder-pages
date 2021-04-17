# Plugin: Neuordnung von Seiten in BrainPress
for WordPress


April 2021

## Short Description 
Gives a (crude) possibility to reorder pages (also called section units) in BrainPress without copy&paste of 
modules.

WARNING: This is tentative software! USE IT AT YOUR OWN RISK!

If you do not use BrainPress, then this plugin is of no use for you and will not work.

## Quick Instructions

Install the plugin by copying the folder brainpress-reorder-pages to the plugin folder 
of your WordPress installation.

Go the the Plugins-page in your WordPress admin area and activate the plugin. There 
are no preferences.

Now you have a new button "Reorder Pages" showing on the admin unit screen of a course 
(more or less) at the left of the tabs of pages. Press the button to reorder these 
pages of of the active unit.

The button "Reorder Pages" brings up a modal window where you can reorder your pages 
by drag and drop. When you are happy with the new order press "Reorder!" in the upper right 
corner of the modal window.

Depending on the number and size of your pages (number of modules) it can take a couple 
of seconds. Afterwards your pages are reordered. 


**CAVEATS:**

1. You **need** BrainPress (testet up to 2.1.0.1) - otherwise your database 
  very likely will be messed up.

2. You **should NOT** reorder pages of courses that have been worked on by students. Their 
   history will get messed up by reordering pages!

3. **Before** reordering pages you have to save your units, otherwise your changes are lost

4. If in a future release the development team of BrainPress Pro changes the data structure of courses, 
   units, pages and modules in the database, then this plugin will no longer work.

5. This plugin works in two phases:   
   in phase (1) it checks if it can change the page order by traversing all affected data. If there is a problem, it will print hints 
   about the problem, but not make any changes. If there are no problems, then   
   in phase (2) the plugin will execute the necessary changes and reload the units page of the 
   course. Now the pages should be reordered. 
   This plugin changes your BrainPress database - there is no "undo"!

## Known Problems

- under some circumstances while moving the boxes of the pages in the modal window, 
  the background can move, too. Boxes might disappear, but appear again, when you release 
  the mouse.

- The plugin is tested on Safari, Firefox and Chrome on Mac. With Safari the modal 
  window sometimes jumps to the left, when you press "Reorder!". Just click the button 
  once more, and it will work.

- If your database was in a doubtful state because of.... *any reason* .... the results 
  can be erratic. Unfortunately there is no easy solution for this problem....  



Thank you for trying!




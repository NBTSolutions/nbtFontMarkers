# nbtFontMarkers
Vector Font Markers for Web Mapping

Adding to this Icon Font:
  1. Create a login for icomoon.io
  2. Open the icomoon app by clicking the red button at the top of the screen
  3. Import the NBTFontMarkers icon set by clicking the purple "import icons" button at the top of the screen and choosing the FontMarkersIcoMoonSet.json file
  4. Add additional icons to this font set by clicking menu icon (ie. the 3 horizontal bars... as if you didn't know) next to the font set name and select "import to this set"
  5. Select an svg file to add to the font
  6. When the new icons are uploaded, corresponding buttons should appear in the font set, click each that you wish to import so they are added to the current selection (all selecteded icons will appear with an orange border)
  7. Click generate font at the bottom of the screen, and save over the /fonts/icomoon font files with the subsequently downloaded files
  8. Before logging out be sure to also download an updated version of the FontMarkersIcoMoonSet.json by clicking on the menu icon (those 3 horizontal bars again) and selecting "download json"---be sure to save this file as FontMarkersIcoMoonSet.json in the main /nbtFontMarkers directory so that we can maintain an up-to-date version of the icon markers font 

Updating the CSS Files
  1. Open the /nbtFontMarkers/fonts/icomoon.svg and copy the unicode id(?) for the newly create icon (it should be something like "&#xe600" and will likely be at the top of the list)
  2. Append a class name to the nbtFontMarkers.css, and nbtFontMarkers.less files that is in the same format as the other font icon classes, but that references the unicode id as the content (note that you with have to format it as an escaped string(?) -- in other words... &#xe600" ---> "\e600"
  3. In the nbtFontMarkers.js file, add an item to the nbtFont markers object that specifies the classname, unicode id and font-family of the new icon

Congrats on your new icon

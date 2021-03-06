ILLUSTRO GADGETS
Version 1.0.0
By iamanai

-----------------------
ABOUT

illustro Gadgets is a skin pack inspired by and based on the AddGadgets.com system monitoring gadgets. It is a
combination of the sleek, beautiful theme of illustro and the functionality of the original gadgets, bringing you
the same information presented in a more easily understandable fashion.

-----------------------
CONTACT

Email: iamanaiofficial@gmail.com
Twitter: @iamanai_

-----------------------
LICENSE AND CREDITS

This software has been released to you under a Creative Commons Attribution-Noncommercial-Share Alike 3.0 License
(http://creativecommons.org/licenses/by-nc-sa/3.0/).

Project leader		iamanai

Contributors		iamanai
			SilverAzide

Special thanks to	SilverAzide
			Kaelri
			jsmorely

-----------------------
CHANGELOG

v1.0.0 - 2016-1-20
Additions:
 - Made some confusing settings more descriptive
 - Added disk capacity warning settings to drives meter settings page
Changes:
 - Changed All CPU Meter name / clock speed settings to reflect v0.8.0 changes
 - Updated changelog date formatting, conforming it to the widely-accepted standard for changelogs
Fixes:
 - Fixed a mistake in the update checker that caused it to not actually display the new version number
 - Fixed small typo in changelog for v0.8.0

v0.8.2 - 2016-1-9
General Additions / Changes:
 - Actually updated HWiNFO plugin to v3.0.0
 - Updated ActiveNet plugin to v2.5.1

v0.8.1 - 2016-1-2
General Additions / Changes:
 - Updated HWiNFO plugin to 3.0.0
 - Removed versionAbsolute variable

v0.8.0 - 2016-1-1
General Additions / Changes:
 - Combined all colors with their alpha values
 - Implemented changing of alpha values using the bars in settings skin color pickers
 - Added custom LUA script to separate RGB values from their alphas
 - Changed coloring mechanics in all gadgets to reflect the above changes
 - Updated update checker to get rid of versionAbsolute variable
 - Moved settings skin readme link to the sidebar, replaced previous location with DeviantArt link
All CPU Meter:
 - Separated CPU name from clock speed, moved clock speed to bottom
 - Fixed 'extra operation' errors
GPU Meter:
 - Added GPU name to single GPU meter
 - Implemented proper settings support for dual GPU meter
 - Added memory controller usage bar
 - Added Shader Clock information
 - Fixed inconsistency with memory fraction on single GPU meter (was bolded, changed to normal)
 - Fixed mistake in Dual GPU Meter that would cause GPU 1's name to display as GPU 0's name instead
Drives Meter:
 - Implemented proper support for long drive names
 - Added drive capacity warnings
 - Fixed more copy/paste mistakes

v0.7.1 - 2015-12-7
Settings:
 - Added ability to middle-click on HWiNFOConfig.inc's file path to reset it to the default value
Bug fixes:
 - Corrected the default value of HWiNFOConfig.inc's file path so it will automatically work on any computer
 - Changed hard-coded file path of the settings skin (for gadget settings buttons) to use #ROOTCONFIG#
 - Fixed a mistake causing the GPU usage and memory usage lines in GPU meter to not display accurately
 - Fixed mistake in Dual GPU Meter that would incorrectly size the background when you hide the line graph
 - Updated v0.7.0's changelog in the readme file to the version currently on the Rainmeter Forums

v0.7.0 - 2015-12-6
UI (all skins):
 - Increased row spacing by 1 pixel, and lowered bars from text by 1 pixel
 - Fixed row relative positioning so the 'rowYOffset' variable actually has meaning
 - Removed hover effect for buttons (it causes too much lag when the gadgets refresh)
 - Slightly repositioned the settings button, to align better with the title text
 - Fixed slight overlap on some of the graphs
 - Made space under the line graphs consistent across the skins
 - Changed bar background color and graph background color to be dimmer
 - Removed "about" button
 - Graph lines are no longer antialiased by default (can be changed back)
Code cleanup:
 - Simplified overly complicated positioning equations
 - Separated out HWiNFO sensor IDs from settings files, combined into a separate file
 - Simplified background, making use of ScaleMargins to eliminate warping and combined into 1 meter
 - Removed AllCpuMeterConfig.lua (unused)
 - Began combining colors and opacities
 - Changed variable naming scheme (again)
Settings:
 - Merged the about skin and all settings skins into new unified skin
 - Added an update checker and external links to the about (now "welcome") screen
 - Added option to disable antialiasing on graph lines (more accurate, but less pretty)
 - Implemented ability to change the location of the HWiNFO config file using RainFile (so you don't
 lose your configs when updating the skin pack)
 - Implemented more coloring options (main font colors, graph backgrounds, buttons, etc.)
 - Changed color selectors to be prettier, and incorporate opacity (heavily based on the one from
 "Circuitrous" by Flying Hyrax)
All CPU Meter:
 - Moved fan info to above CPU cores, changed to regular display (label, percentage, value, bar)
 - Moved CPU clock to top, separated from fan speed
 - Added CPU name to top-right, can be disabled individually from clock speed in advanced settings
 - Fully removed support for CoreTemp and SpeedFan
Network Meter:
 - Increased opacity of arrows to match those on Drives Meter
GPU Meter:
 - Added memory used / total memory fraction to the memory usage row
 - Added dual GPU meter variant (select from rainmeter's context menu)
 - Fixed copy/paste error in the metadata section
Drives Meter:
 - Fixed flaw in the line graph that would cause a line to not scale itself in relation to the other
 lines

v0.6.3 - 2015-11-6
Readme.txt:
 - Backported v0.7.0-d.4 format updating to be more aesthetically pleasing on GitHub
 - Reworded some things
 - Fixed changelog dates to be "normal"
Drives Meter:
 - Backported fixes from v0.7.0-d.2 to correct copy/paste errors with the L drive's meters

v0.6.2 - 2015-10-10
Drives Meter:
 - Fixed more mistakes that broke the functionality of the E drive's information

v0.6.1 - 2015-10-9
Drives Meter:
 - Corrected some copy/paste errors made when creating meters for E drive

v0.6.0 - 2015-10-4
Drives Meter:
 - Shows Name, Disk Read Time Percentage, Read/Write Speeds, and storage used / capacity for each hard drive or
 removable disk connected to slots C-L
 - Will automatically adjust when you plug in/unplug a drive, changing the size of the skin to accomodate for
 the new information
 - Line graph shows read/write activity for each disk
 - Histogram shows read/write time (also displayed by the percentage across from the disk's name)
 - Settings let you show/hide the line graph or histogram, select if you want to hide certain drives, and customize
 colors
Code Cleanup:
 - Cleaned up All CPU Meter's main section code, placing meters by row rather than by type
 - Removed All CPU Meter's support for CoreTemp and SpeedFan in favor of HWiNFO
 - Added more settings to Network Meter and GPU Meter
 - Fixed mistake in GPU Meter's settings skin that broke middle-click-to-default functionality for the checkboxes
 - Preparation for mass code cleanup to take place in v0.7 and v0.8

v0.5.1 - 2015-9-13
All CPU Meter:
 - Added support for HWiNFO core temps and fan speed
 - Implemented HWiNFO configuration into settings skin
 - Made all color options always visible (HWiNFO settings made it extremely difficult to adapt per-CPU)
Code Cleanup:
 - Merged core temp meters, cutting 16 extraneous meters from the All CPU Meter skin
 - Began optimizing code, in preparation for final release and to make drives meter easier to implement
Notes:
 - Auto-detection of system monitoring software is currently broken. Implemented a temporary workaround in
 All CPU Meter's settings skin

v0.5.0 - 2015-9-12
GPU Meter:
 - Monitors your graphics card usage, clock speed, temperature
 - Gives information about memory clock speed, memory usage, fan speed and usage, memory controller usage,
 and core voltage
 - Requires HWiNFO
 - Settings skin has tools for configuring the skin to work with HWiNFO as well as color customization

v0.4.1 - 2015-8-20
Changed how Network Meter reads the internal I.P. address (It is now REQUIRED to have Rainmeter 3.3 Beta
installed to make this work properly)
Fixed a flaw with All CPU Meter that messed up snapping other skins below it.

v0.4.0 - 2015-8-19
Code cleanup:
 - Created a global variables .inc file to share variables between skins
 - Moved more positioning numbers to variables for easy debugging
 - Got rid of unneccesary variables
 - Simplified background positioning
General UI Cleanup:
 - Changed button code to be more clickable and include a fancy visual change when hovering over a button
 and clicking on it
 - Increased resolution of images and used Rainmeter to downscale them, increasing quality and preparing
 for future features
 - Changed color of graph background and color customization number input backgrounds to be more visible
 - Added degree symbols to the core temperatures (I was using the wrong file format for the skin files,
 so these weren't possible before)
All CPU Meter:
 - Changed behavior of opening task manager to a double-click anywhere on the gadget
All CPU Meter Settings:
 - Added the ability to show/hide the graph, as well as show/hide the clock and fan speed info
New "About" skin:
 - Gives information about the skin pack
 - Provides a link to the Readme file
ActiveNet Plugin:
 - Added the ActiveNet Plugin for use with Network Meter
 - Requires .NET Framework v4.5 or later to function properly
Network Meter:
 - Added Network Meter (uses the ActiveNet Plugin)
 - NOTE: To configure the Network Meter, follow this link: http://comments.deviantart.com/1/522574269/3808722511

v0.3.0 - 2015-8-5
Added support for core temperatures using CoreTemp or SpeedFan
Some code cleanup
Implemented settings skin (incomplete)
Settings:
 - Show/hide page file info
 - Show only average CPU usage on the graph
 - Show/hide core temperatures
 - Choose either Fahrenheit or Celsius for core temps
 - Customize colors of each bar and its corresponding line on the graph

v0.2.0 - 2015-8-2
Added All CPU Meter

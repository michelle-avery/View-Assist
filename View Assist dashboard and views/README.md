This is a list of things to do and things done for the dashboard/ui upgrade

# To do

* Incorporate proof of concept icon handling automation into device configuration blueprint
* Insure icon list is always defined.  Do this either in device configuration blueprint on startup, device configuration default or handle in icon handling sequences (aka update jinja to handle)
* Add new VA Assist listening CSS
* Look at both assisting and processing variants of the bar and popup
* Add select for listening CSS preference to device configuration blueprint.  Choices are new (default) and existing bar
* Add select for microphone type (Stream Assist, HASSMic, Home Assistant voice satellite, other) to device configuration blueprint
* Use microphone type to set variables in variable template
* Update all existing full screen views to take up all available space
  * Alarm - use absolute positioning for snooze and dismiss buttons
  * Weather - also look at clipping
  * Music - alternative done (?)
  * Sports
  * All Cameras (custom)
  * Camera
  * Webpage
  * Thermostat - also look at making larger
* Consider option to handle icon bar list color (black or white) OR figure out how to add drop shadow on icons to ensure viewable on white backgrounds
* Test launch icons in status bar
* Add option to device configuration blueprint to allow users to set launch icons.  These will be added to the list on start up and never removed
* Document how to add button template for custom icons
* Document how to manipulate icon lists for developers
* Add ability to set default background in device configuration blueprint and use in clock card
* Look at setting default dashboard in VA device config so things like buttons can be more dynamic


# Done

* Change method for displaying icons using VA device attribute status_icons list (thanks @JimmyJamesBob)
* Proof of concept automation for adding/removing default icons (mic mute, speaker mute, do not disturb, hold mode)
* Test proof of concept icon display and automation with at least one user (thanks @JimmyJamesBob)
* Move existing bar to bottom of screen
* Set default z-index level for title and status areas so they are always above main card
* Update all existing full screen views to take up all available space
  * Clock - use absolute positioning for date and time  
  * Locate
  * Music - default done (thanks @JimmyJamesBob);
  * List (no change needed)
  * Intent (no change needed)  
# Walker

<span style="display:block;text-align:center;">![Walker](supporting-files/screenshots/hero.png)</span>

A free data field for Garmin watches to provide stats for walking activities. Built to provide more data in a more compact format than is typically available on data fields designed for runners (where too much information becomes impossible to digest at speed). Focused on data relevant to casual walking scenarios where step count, distance, pace and calorie burn are the predominant concerns rather than hiking where bearing, ascent and altitude etc. are more relevant. Currently displays:

- Clock time
- Average pace or speed for the current activity (controlled by settings)
- Total distance for the current activity
- Current pace or speed (or rolling 3/5/10/30/60 second average by changing settings) *
- Total time for current activity
- Current heart rate (or rolling 3/5/10/30/60 second average by changing settings) *
- Current heart rate zone and heart icon coloured by zone (if enabled in settings - disabled by default)
- Steps for the current activity
- Steps for today
- Calories for current activity
- Calories for today
- Battery charge level with colour changing battery icon
- Progress bar showing progress towards step goal (if step goal is set)

* 3, 10, 30 and 60 second modes disabled on some older devices due to memory constraints

Walker also contributes step data to the FIT profile for your activity, showing total steps, lap steps and average steps per km/mile/hour in the activity summary in Garmin Connect. It is aware of and supports device settings for distance units (KM or miles), background colours (black or white), and 12/24 hour clock mode. Feature suggestions are welcome and will be considered.

<span style="display:block;text-align:center;">
	![Screenshot 1](supporting-files/screenshots/screenshot-1.png)
	![Screenshot 2](supporting-files/screenshots/screenshot-2.png)
	![Screenshot 3](supporting-files/screenshots/screenshot-3.png)
	![Screenshot 4](supporting-files/screenshots/screenshot-4.png)
	![Screenshot 5](supporting-files/screenshots/screenshot-5.png)
</div>

## Installation
Installation and setup of data fields on Garmin watches is not as straightforward as one might hope. Once you know the procedure it us a fairly quick process, and hopefully these step-by-step instructions will make it easy to follow. These instructions are confirmed to work correctly with my own watch (fenix 5X) and should be broadly applicable to most Garmin watches, but steps or button layout may vary by watch model.
1. Go to [https://apps.garmin.com/en-US/apps/6cfd1ea6-e841-4c6a-98d2-b87a0b68ee74](https://apps.garmin.com/en-US/apps/6cfd1ea6-e841-4c6a-98d2-b87a0b68ee74) in a web browser and (after logging in with your Garmin account) press the "Download" button.
	- You will be asked which device you want to install to.
	- Select the device from the dropdown list and press "Confirm Device".
2. Alternatively, search for "Walker" in the Garmin **ConnectIQ** app on your phone, select Walker by wwarby from the search results and press "Install".
3. Sync your device using the Garmin **Connect** app
4. Once the sync is complete, the Walker Data Field is installed on your phone, but you must also assign it to the sporting activities on which you want to use it.
	- Typically with will be for the "Walk" activity so the instructions that follow are for the "Walk" activity, but you may also want to repeat these steps for "Hike", "Treadmill" etc. or for older watch models that don't have the "Walk" activity you might want to use the activity type "Other".
5. Starting from the watch face, press the top right button. That should display the list of available activities.
6. Use the bottom left button to scroll down until “Walk” is highlighted in bold
7. Press and hold the middle left button. You should see a menu with “Walk Settings” highlighted.
8. Press the top tight button to enter the “Walk Settings” menu. You should then be in a sub-menu with “Data Screens” highlighted.
9. Press the top tight button to enter the “Data Screens” menu. You should now see a data screen with a pencil icon in the top right.
10. At this point you can scroll up and down through the data screens you already have configured for Walk activities using the middle left and bottom left buttons. Scroll down to the end of the list using the bottom left button and you should see a screen with a big green + and the words “Add New”
11. Press the top right button to add a new Data Screen. You should land in a menu with “Custom Data” highlighted.
12. Press the top right button. You should be asked to “Choose Layout”, where you’ll be able to scroll up and down through different layouts. You want the top one, which just has “Field 1” in the middle.
13. Press the top right button to move to choosing the field. You should land in a menu with Connect IQ Fields highlighted and 0/2 Added underneath.
14. Press the top right button. You should land in another sub-menu, where you’ll be able to select the downloaded data field you want to use.
15. Scroll down using the bottom left button until “Walker” is selected, then press the top right button to select it.
16. You should now see the Walker data field on your screen, but it will be the last data field in the list. You probably want it to be the first so that it shows by default when you start a walk.
18. Press the top right button to edit the position of the field. You should land in a menu with “Layout 1 Field” highlighted. Use the bottom left button to scroll down to “Reorder”
19. Press the top right button. You should now land in a sub-menu where “Walker” is highlighted.
20. Press the middle right button repeatedly to move Walker up to the top of the list, then press the top right button to confirm.
21. You’re done. Press the bottom right button three times to exit out of the menus, and you should be back to the activity selection menu with “Walk” selected.
22. Press the top right button to select the “Walk” activity and you should find you’re ready to go for a walk with Walker shown on screen by default.

## Supported Devices
- Approach S60 / S62
- Captain Marvel / Darth Vader / First Avenger / Rey
- D2 Bravo / Bravo Titanium / Charlie / Delta / Delta PX / Delta S
- Descent Mk1
- fenix 3 / 3 HR / 5 / 5 Plus / 5S / 5X / 5X Plus / 6 / 6 Pro / 6S / 6S Pro / 6X Pro / Chronos
- Forerunner 230 / 235 / 630 / 645 / 645 Music / 735xt / 935 / 945
- MARQ Adventurer / Athlete / Aviator / Captain / Commander / Driver / Expedition / Golfer
- Venu
- vivoactive 3 / 3 Music / 3 Music LTE / 4 / 4S

*Note: Only tested in on a real fenix 5X in the field, all other watches tested only in the SDK device simulator.*

## Supported Languages
- Arabic
- Bulgarian
- Chinese (Simplified)
- Chinese (Traditional)
- Croatian
- Czech
- Danish
- Dutch
- English
- Estonian
- Finnish
- French
- German
- Greek
- Hebrew
- Hungarian
- Indonesian
- Italian
- Japanese
- Korean
- Latvian
- Lithuanian
- Malay
- Norwegian
- Polish
- Portuguese
- Romanian
- Russian
- Slovak
- Slovenian
- Spanish
- Swedish
- Thai
- Turkish
- Vietnamese

### Note on language support in the Garmin simulator
Arabic, Hebrew and Thai supported by the Garmin ConnectIQ SDK but are not rendered correctly in the device simulator. The simulator also seems to throw an exception when a Thai string resource is used for the units of a FIT contribution. I have tested Arabic and Hebrew on a real fenix 5x watch and it seems to work fine, but my watch doesn't support Thai. Due to these issues it is impossible for me to thoroughly test these languages on all devices.

### Translation help
Help with internationalisation would be appreciated. Current translations are based on Reverso and Google Translate. I've made an effort to find the correct translations but have no easy way of finding out if they are correct except through user feedback.

## Source
Walker is open source (MIT license) and it's code resides on GitHub at https://github.com/wwarby/walker

## Credits
Code and ideas borrowed from [RunnersField by kpaumann](https://github.com/kopa/RunnersField) and [steps2fit by rgergely](https://github.com/rgergely/steps2fit). Thanks for open sourcing your projects.

### Icon Credits
- Icons by [Freepic](https://www.flaticon.com/authors/freepik) from [www.flaticon.com](https://www.flaticon.com)
- Flame icon by [Those Icons](https://www.flaticon.com/authors/those-icons) from [www.flaticon.com](https://www.flaticon.com/free-icon/fire_483675)

## Changelog
- 1.0.5
  - Removed "BETA" from the app name
- 1.0.4
  - Fixed where I accidentally left screenshot hard-coded values in the build
- 1.0.3
  - Increase font sizes for Forerunner 230, 235, 630 and 735XT
- 1.0.2
  - Fix calculation bug when speed display mode was selected
- 1.0.1
  - Add Arabic, Hebrew and Thai language translations
- 1.0.0
  - Add FIT contributions for average steps per km/mile/hour
  - Smaller heart icon when HRZ is disabled
  - Show + or - if HR is outside HR zones
  - Memory optimisation
  - Add language support for all remaining languages supported by Garmin
- 0.6.3
  - Fix bug where incorrect heart rate zone was shown
  - Fix bug where speed was calculated incorrectly if units were set to miles and speed display was enabled in settings
  - Fix bug where pace units setting on watch was ignored (distance units was being used for pace)
- 0.6.2
  - Fix bug with duplicate label in settings
- 0.6.1
  - Accurate French and Russian translations
- 0.6.0
  - Fix missing settings
  - Add setting to show speed instead of pace
  - Added support for several new languages
- 0.5.0
  - Use larger fonts where possible on all devices
  - Make daily steps and calories text darker on white backgrounds
  - Add support for new watch models
- 0.4.1
  - Fix battery icon position bug on 240x240px screens
- 0.4.0
  - Add heart rate zone (configured by setting, disabled by default) to heart icon
  - Colour heart icon by heart rate zone
- 0.3.0
  - Add FIT contribution for steps
  - Support for "resume later" on activities
  - Localised language support for several European languages
  - Fix bug that would reset activity steps on activity "stop" (as opposed to "reset")
  - Memory usage optimisation
- 0.2.0
  - Add step goal progress bar
  - Hopefully support stable transition across midnight boundary for step counter
  - Optimised images for compression efficiency
  - Screenshots for Garmin Store
- 0.1.0
  - Initial alpha release

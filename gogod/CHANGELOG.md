# Changelog

### Version 2.1.8 - 2017-06-21
* Improved performance
* Reduced bugs
* Added features like QR Code on webUI 

### Version 2.1.5 - 2017-06-21
* Updated IFTTT link in setting page.

### Version 2.1.4 - 2016-12-18
* Added a new class of rate limit checking.
* Updated Data Log View to show marker if the number of points is less than 100.
* Fixed a Data Log issue when add a new point.
* Fixed addons error.
* Updated Web UI to prevent right click

### Version 2.1.3 - 2016-11-28
* Fixed Telegram Bot issue.
* Added rate limit to each cmd Packet
* Updated IFTTT description in setting page

### Version 2.1.2 - 2016-08-18 - Marutpong Chailangka
* Added photos display on the data logging graph
* Updated loading data logging from each file directly for better performance.  

### Version 2.1.1 - 2016-08-04 - Marutpong Chailangka
# Fixed issue when show current image on Pi Display

### Version 2.1.0 - 2016-08-03 - Marutpong Chailangka
* Added IFTTT Trigger
* Added Telegram Bot to send message and image
* Added Pi Display Text-to-Speech Configuration
 * replaced speech synthesis engine to ResponsiveVoice JS
 * supported multi-browser
 * supported to change voice, pitch and rate
* Updated more media file types supported (for pi display and file downloading)
* Added console logging and log by pattern (date title message)
* Added auto correction of media file name
* Fixed SMS Sending issues
* Fixed wifi issue

### Version 2.0.0 - 2016-07-05 - Marutpong Chailangka
* Added support send topic/message from GoGoBoard to Raspberry Pi
* Updated add-ons functions
 * Added functions to get/save variables from/to a file
 * Added a function to correct filename (remove special characters)
 * Added a function to run activated add-ons automatically
 * Changed add-ons filename to example.py

### Version 2.0.0(Beta 2) - 2016-07-04 - Marutpong Chailangka
* Added configuration of logging
* Add-ons
 * Added checking file exists in verify API
* Data logging
 * Added a API to log a record
 * Added a API to get the records in JOSN format by append '.json'
 * Changed getting log records API from  'fetch' to 'get'
 * Changed  fail to upload queue from variable to a file 
 * Updated handling the queue and normal logging
 * Updated method of sending to server by using the requests module
 * Updated log display by setting dynamic height
* Updated a checking token method in PushBullet

### Version 2.0.0(Beta) - 2016-07-01 - Marutpong Chailangka
* Updated html rendering from PHP to python (Tornado) except filemanager
* Updated serving PHP by itself standalone (port 8889) instead of using Apache
* Added REST API
  * key-value 
  * datalog management
  * wifi connecting
  * configuration 
  * add-ons functions
* Added GoGoD Addons Interface (both Python module and WS at http://{ip}:8888/ws_interface), sending and receiving the key-value packets between GoGo Board and Raspberry Pi
* Updated data logging : logging to csv file by default and removed other dependencies (such as orientDB)
* Updated wireless : supported enable/disable auto connecting

### Version 1.1.1 - 2015-03-16 - Marutpong Chailangka
* Updated Pushbullet configuration

### Version 1.1.0 - 2015-12-12 - Marutpong Chailangka
* Fixed logging to file bug.
* Improved cloud data logging.
* Added a feature to Cloud data logging. When unable to logging, it will store to queue and handle logging to server later.
* Fixed updating Cloud API key issue.

### Version 1.0.7 - 2015-11-28 - Marutpong Chailangka
* Improved cloud data logging

### Version 1.0.6 - 2015-11-26 - Marutpong Chailangka
* Added a feature : showing recently image when open Pi Display

### Version 1.0.5 - 2015-11-18 - Marutpong Chailangka
* Added a feature : Cloud data logging at https://data.learninginventions.org by rate limited (5s)
* Updated : database logging by rate limit 0.5 seconds

### Version 1.0.4 - 2015-10-10 - Marutpong Chailangka
* Updated the Web UI view to hide the edit button and new button on small screen.
* Fixed wifi issue.
* Replaced handling the value of data recording command as string.
* Updated data logging to limit the logging rate.
* Added a feature : Deleting the logged datas.
* Updated the layout of each page.


### Version 1.0.3 - 2015-08-21 - Marutpong Chailangka
* Added RIB (Rapid Interface Builder) to GoGo Home Screen
* Added a feature : Export from Rapid Interface Builder to Web UI
* Added a feature : Import from GoGo to Rapid Interface Builder
					(The Web UI html files can be edit)
* Added a config python class with read/write method and recoded handling the config
* Added a feature : Auto connecting to wifi
* Added a feature : Speech recognition is supported Thai Accent
* Show the version of Gogod on the top of GoGo Home Screen
* Updated the Web UI example files
* Replaced WebSocket with ReconnectingWebSocket
* Improved data logging methodology by integrated a queue
* Improved Speech Recognition to handle the speech when tapped it

### Version 1.0.2 - 2015-08-14 - Marutpong Chailangka
* Fixed USB Wifi (TP-Link)

### Version 1.0.1 - 2015-08-04 - Marutpong Chailangka

* Fixed Web UI to support utf-8
* Added Local Rapid Interface Builder
* Updated path of snapshot(can access via file manager and pi display)
* Fixed a data logging issue, can't log data to DB

### Version 1.0 - 2015-07-22 - Marutpong Chailangka
Features
* Pi Display (play sound, show image)
* File Manager
* Data Logging (sensor logging, graph)
* Sound Recording
* Web UI (using the html elements to control the GoGo Board)
* Speech Recognition
* Web Services
  * Email Sender
  * IFTTT, Pushbullet
* Web Camera (take snapshot, face detection)
* USB Devices
  * SMS Sender
  * RFID Reader/Writer

Update
* Major change of UI and functions
* Updated Responsive File Manager
* Used same algorithm to encrypt the password in python and PHP
* Replaced a text config file by a json file 
* Hidden a debugging message in Push
* Fixed the menu bar when display on meduim screen size
* Fixed setting icon
* Fixed filling extention of sound record files
* Fixed saving email config status
* Fixed text-to-speech to prevent gogo suspending
* Bug fixes

Add
* Missing the descriptions in UI and code
* Offline jQuery qrcode generator
* Setting page (Pushbullet Token, Email Account)

 

Quotes Display Apps Functional Specification V2.1
=================================================

## Project Goal
---
To display personal/book quotes in your Android device. The quotes are 
to be read from text file(s) and displayed (one by one) in random order 
at periodic intervals (or on screen-tap). 

We have two applications: 

* **Random Quotes App:** Application to turn an Android device into a 
"picture frame" for displaying quotes.

* **Random Quotes Widget:** Application to display the quotes in a small widget 
in the Android device front screen. 

## Use Cases.
---

A person has a text file with some paragraphs(quotes) or notes he/she has 
made (life quotes, book summaries ...etc).

### A house picture frame

He would like to put his quotes in a digital picture frame for displaying 
them in the house/apt ...etc. He uses an old android phone as a picture 
frame and installs the Random Quotes Application to display a random quote 
every hour.

### A personal reminder.

She would like to keep her favorite quotes in her cell-phone and display 
a new quote on-tap. She installs the Random Quotes Widget and places 
the widget in her home screen.

## User Features & Issues to Solve
---

* One **major feature per major release**: v1, v2, v3 ...etc.
* Minor features and bugfixes are minor releases: v1.1, v1.2 ... etc

### Random Quotes Widget

* Create Widget Logo.
    SVG -> multiple .png sizes.
    > Done.

* Add support to scan directories.  
    Support for scanning diretories and populating the book summaries 
    list, so that you dont have to select file by file.  
    > Done.

### Random Quotes Libraries.  

* Add support for integrated file/dir choser library.  
    aFileDialog  
    > Done.  

### Random Quotes Application.

* Create App Logo.
    SVG -> multiple .png sizes.
    > Done.

* Add support to scan directories.
    Support for scanning diretories and populating the book summaries 
    list, so that you dont have to select file by file.  
    > Done.
    
* Add support to select daytime start & end time.  
    When the picture frame turns on. When the frame turns off.  
    > Done.
    
* Add support for variable quote display updates.
    1min, 5 mins, 30 mins, 60 mins ...etc.
    > Done.

## Posponed Features.
---

**Potentially unnecessary**, postponed for later consideration. 

### Random Quotes Widget

* User Wiki (v2.3).
    For public collaboration.

* Add support for variable widget updates (v2.2).  
    Based on an alarm utilities library.

* Add support for different fonts/sizes (for different screen devices) and background colors (v2.2).

### Random Quotes Libraries. 
* Implement Alarm Utilities Library (v2.2).
    Functional interface around alarm manager. Support for inexact RTC 
    timing. 
    
* Implement Errata Library Functionality (v2.2)  
    On tap add current quote information to text file.  
    To ease noting which quotes need to be fixed in the future i.e. when going over the errata text file.  
    
* Implement Database Storage Library (v3.0)
    Change backend storage from SharedPreferences to SQLite.  
    While unnecessary today, it could be nice when working with large 
    numbers of text files. 

### Random Quotes Application.

* User Wiki (v2.3).
    For public collaboration.

* Add support for different font and background colors (v2.2).

* Add support for precise Daytime events (v2.3).  
    Make daytime check based on alarm events, not tied to periodic updates.  
    e.g. starting handler updates and turning ON the screen exactly at 
    the user-chosen start_daytime. Stoping updates and turning the 
    screen OFF at the user-chosen end_daytime.
    
## Removed Features.
---

**Completely unnecessary**, remove from further consideration, purge 
from future specs.

* Open text file directly from view.  
    Could be nice when integrated with a third-party text editor and 
    server synchronization (unison?).  
    > Postponed: Not currently necessary/practical. 

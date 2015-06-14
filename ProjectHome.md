# Description #
I've found myself loosing a lot of time with creating drawables in different density sizes. The Android Drawable Converter project intents to help you by supplying a tool that is able to convert drawables into other density versions like ldpi, mdpi, hdpi, xhdpi automatically.

# Installation #
To use this project you can download "Android Drawable Converter V2.0.0" on the download page.

This project needs imagemagick to convert the drawables so make sure you have imagemagick installed: http://www.imagemagick.org/script/binary-releases.php.

  1. Create your drawables in the highest density you need.
  1. Fill out the **settings.ini** (Most important **convert\_command**, **convert\_source** and **convert\_destination**).
  1. Move the **android-drawable-converter.jar** and **settings.ini** to the **root** of your android project or supply the **convert\_source\_path** and **convert\_destination\_path** options to convert an absolute source directory to multiple absolute destination directories.
  1. Execute "**java -jar android-drawable-converter.jar**"
  1. **You are done** all the drawables from the convert\_source to all convert\_destinations have been created.

# Options #
  * You can use all the parameters in settings.ini as arguments when executing android-drawable-converter.jar. Ex: "java -jar android-drawable-converter.jar convert\_destinations ldpi"
  * You can supply multiple convert\_destinations like "convert\_destinations=ldpi,mdpi,hdpi"
  * Technically you could use this tool for iPhone by defining your own formats and defining the convert\_source\_path and convert\_destination\_path in the settings.


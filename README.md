# RikiApp

###### Prepare your distro for compile:

+ Download Android Studio from https://developer.android.com/studio/index.html#linux-bundle
+ Extract the zip file into a folder at your home dir(i.e. android_ide) and run the bin/studio.sh script
+ Select Standard setup and finish the installation.
+ When the download is done, press on the Configure option on the bottom side and select SDK manager
+ From SDK platforms select all API levels from 26 to 22
+ From SDK Tools select 'Show package details'
+ Select 21.1.2 ,25.0.2 and 26.0.0
+ Press apply and ok
+ Accept the license and let it download the required files
+ Press ok to SDK manager and close the Android Studio
+ Install the JDK8 by running 
> $ sudo add-apt-repository ppa:openjdk-r/ppa  
$ sudo apt-get update  
$ sudo apt-get install openjdk-8-jdk

+ Run the android studio: . /path/to/studio/bin/studio.sh
+ File->Open->RobotCA/src/android_foo folder and press OK.
+ Wait until Gradle is being initialized.
+ On the plugin update window,select "Dont remind me again for this project".
+ File->Other Settings->Default Project Structure->Untick default JDK and add this directory: /usr/lib/jvm/java-1.8.0-openjdk-amd64
+ Close Android Studio and run 
> $ sudo apt-get install lib32z1 lib32ncurses5 lib32stdc++6

+ Open Android Studio again and wait gradle to be initialized


Dependencies:  
+ ROS
+ ROSJava
+ Android 4.0+ (API level 13+)

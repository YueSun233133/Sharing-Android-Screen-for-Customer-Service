Sharing Android Screen for Customer Service

## Description
This is an android app that allows customers who need help with their mobile devices to connect directly with our service providers, the aim for this project is to establish peer to peer screen sharing, but so far we have only accomplished peer to peer camera sharing, and we are trying our best to figure out a way to change our sharing from camera to screen, but this is extremely hard and we have tried dozens of ways that doesn't work. Besides from this, our other functions just works fine, you can start the app, login or register, then you'll come to our profile page, which will display your username, your email information, you can change password and logout in this page, and also press the assistance button to initiate direct peer to peer video chat with pc.

If you are doing a project review, the following instructions will guide you to use our app, for any questions, please contact Wenpeng Wang, +1-(857)8005627.

## Instruction(Please follow this instruction to implement this app)

* git clone https://github.com/YueSun233133/Sharing-Android-Screen-for-Customer-Service.git
* Open an existing Android Studio Project Sharing-Android-Screen-for-Customer-Service-master/AndroidRTC-android-studio-sprint3
* Run this application in Android Phone
* Using Firefox browser to open the link:http://35.161.177.232:3000/ and click "Start" buttom to share screen on PC
* Launch app on your android phone and register and log in and start to share screening by click "copy to the clipboard"
* click "Refresh" buttom on browser and click call then you can start to share screen!


## ProjectRTC

- Node.js server
- Desktop client
- Android client

The signaling part is done with [socket.io](socket.io).
The client is built with [angularjs](https://angularjs.org/).

## Install

It requires [node.js](http://nodejs.org/download/)

* git clone https://github.com/YueSun233133/Sharing-Android-Screen-for-Customer-Service.git
* cd Sharing-Android-Screen-for-Customer-Service/ProjectRTC/
* npm install
* npm start

The server will run on port 3000.
You can test it in the (Chrome or Firefox) browser at localhost:3000.
 
## AndroidRTC
(https://chromium.googlesource.com/external/webrtc/+/master/webrtc/api/android/java/src/org/webrtc)

An Android client for 

It is designed to demonstrate WebRTC video calls between android devices and desktop browsers, but WebRtcClient could be used in other scenarios. 

* git clone https://github.com/YueSun233133/Sharing-Android-Screen-for-Customer-Service.git
* open exist project in Android Studio Sharing-Android-Screen-for-Customer-Service/AndroidRTC-android-studio-sprint3/
* change ../app/res/values/strings.xml "<string name="host">35.161.177.232</string>"
* change ../app/java/fr.pchab.androidrtc/utils/Constant, public static final String BASE_URL = "http://35.161.177.232:8080/api/v1/" 
  

## How To

ProjectRTC should be on and running, and it must be somewhere that your android can access. Modify the host to the server IP.(command: ifconfig | grep inet)

Your stream should appear as "android_test" in ProjectRTC, so you can also use the call feature there to communicate with pc.



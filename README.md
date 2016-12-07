Sharing Android Screen for Customer Service

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
* change ../app/res/values/strings.xml "<string name="host">YOUR IP ADDRESS</string>"
* change ../app/java/fr.pchab.androidrtc/utils/Constant, public static final String BASE_URL = "http://YOUR_IP_ADDRESS(10.0.2.2):8080/api/v1/" (10.0.2.2 for virtual device, YOUR_IP_ADDRESS for real Android Device)
  

## How To

ProjectRTC should be on and running, and it must be somewhere that your android can access. Modify the host to the server IP.(command: ifconfig | grep inet)

Your stream should appear as "android_test" in ProjectRTC, so you can also use the call feature there to communicate with pc.



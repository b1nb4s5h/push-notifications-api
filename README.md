<p align="center">
<img src="https://i.imgur.com/aO2e1bD.png" width=128 align="center">
</p>

<p align="center">
<b>Push Notifications API</b>
<br>
Version: <b>1.1.1</b>
</p>

# About
Push Notifications API is a simple Android app for displaying notifications on your phone through a REST-API.  
It is a tool for developers that need a easy way to post notifications on their phone. The application requires an API to handle all the notifications. There is a working example of a Python REST-API in the [api](https://github.com/viktorholk/push-notifications-api/tree/main/api) folder that works with the Android app. You can customize the API to your liking.  
The application  is great for IoT (Internet of Things). You could for example post a notification to your phone every time your garden needs watering when a sensor has detected the level of soil moisture to be low. The possibilites are up to you!  

You can download the Android app through [Google Play](https://play.google.com/store/apps/details?id=com.viktorholk.apipushnotifications) or download the latest apk from the [releases](https://github.com/viktorholk/push-notifications-api/releases).
# Usage
<p align="center">
<img src="https://i.imgur.com/bUojChY.png" width=256 align="center">
<img src="https://i.imgur.com/ApgZyKL.png" width=256 align="center">
</p>

* Configuration  
In the configuration tab, you can configure the endpoint which the application will listen to for the notifications.  
You can edit the poll time for each request to spare your phone's battery.
* Service  
In the service tab, you can toggle the notification service.

# Create a notification:

curl --request POST \
  --url http://xxx.xxx.xxx.xxx:5000/notifications \
  --header 'Content-Type: application/json' \
  --data '{
  "title": "ThisIsTheTitle",
  "body": "Here are some body text for the notification"
}'


## Issues
Please report issues using [GitHub's issues tab](https://github.com/viktorholk/push-notifications-api/issues).


## License
Push Notifications API is under the [MIT LICENSE](LICENSE).


# Jamun-Camera

Camera library provide you Custom Complete Camera view with full features like Flash, Rotation, Gallery Picker, Focus, Tap to capture, Confirmation window and last but not least croping feature. It also provide you file path in return so that developer can feel a friendly handy way to Deal After. 

### What's New? {Latest Version}
* Stable **Official Version** for Developers and Live Apps.
* Easy Calling Mechanism with **Instant reply** via onActivityResult.
* Need less calls with many customs Tags in Intent Object to reach maximum developer satisfaction.
* Compatible With **[Gallery](https://github.com/Lib-Jamun/gallery.git)** Library for More Efficent Working;
* App with continous face Detaction Feature.

### Why this library?

* This library Competible with all screen sizes and device (Tab with 7' inches and 10'inches).
* Library support both orientation that is portrait and landscape.
* Its Calling feature is very simple and easy to use.
* You don't need to add Multiple libraries and UI components, It have such Components inside that make Quality.
* Library is Customizable for **Enable Gallery Mode** or **Only Camera Mode** .
* Library Automaticaly Handle Flash, Rotation and Focus mode Availablity that is Device Dependent.
* Library **Doesn't force App Camera Dependent** Feature in Playstore Device Compatible Analogs.

### Quality Measures? for {Latest Version}

The following apps are using this library without facing any kind of Bugs.

* **[SimplyBlood](https://play.google.com/store/apps/details?id=com.simplyblood)**
* **[ZINI](https://play.google.com/store/apps/details?id=ai.zini)**,
* **[RentalBazar](https://play.google.com/store/apps/details?id=com.rentalbazaar)** 
* **[DoubtCrusher](https://play.google.com/store/apps/details?id=com.doubtcrusher)**
* **[BookAGround](https://play.google.com/store/apps/details?id=com.bookaground)**
* **[PeyFree](https://play.google.com/store/apps/details?id=com.peyfree)**
* **[ClueRace](https://play.google.com/store/apps/details?id=com.cluerace)**
* **[CIS-Connect In Single](https://play.google.com/store/apps/details?id=com.connectinsingle)**
* **[QR/Barcode Scanner](https://play.google.com/store/apps/details?id=com.scanner.android)** 
* **[Wall-E](https://play.google.com/store/apps/details?id=com.walle.android)**

------

### Jamun-Camera Preview

Window View | Working Preview
---- | ----
![jamun_camera](https://user-images.githubusercontent.com/38988514/40282370-fddb9780-5c8b-11e8-9124-6008eb15dbc1.png) | ![jamun_camera](https://user-images.githubusercontent.com/38988514/40282466-6ede2fb4-5c8d-11e8-958c-4366adc114af.gif)


### Gradle Configuration

**Add the dependency**

Step 1\. Add the jCenter repository to your build file. Add it in your root build.gradle at the end of repositories:

```java
allprojects {
  repositories {
        mavenCentral()
  }
}
```

Step 2\. Add the dependency

```
Latest Version : 0.0.8

Android
dependencies {
     compile 'tk.jamun.ui:camera:{Latest Version}'
}

AndroidX
dependencies {
     compile 'tk.jamunx.ui:camera:{Latest Version}'
}

Kotlin
dependencies {
     compile 'tk.jamun-ktx.ui:camera:{Latest Version}'
}
```

### Maven Config

```xml
<dependency>
Android
  <groupId>tk.jamun.ui</groupId>
AndroidX
  <groupId>tk.jamunx.ui</groupId>
Kotlin
  <groupId>tk.jamun-ktx.ui</groupId>
  <artifactId>camera</artifactId>
  <version>{Latest Version}</version>
  <type>aar</type>
</dependency>
```
------
### How to Implement

Once the project has been added to gradle, You can use these lines of code to configure pickers....

#### Step 1. Define Intent Object

Simple Object declaration :

```
Intent intent = new Intent(this, ActivityCamera.class);

```
#### Step 2. Start Module By Calling

This method is very common to Android Developer, Very easy calling way to Start an activity help you same for calling this Picker :

```
startActivityForResult(intent, ACTION_REQUEST_CAMERA);

```

#### Step 3. Get Result from Picker

```
@Override
public void onActivityResult(int requestCode, int resultCode, Intent data) {
super.onActivityResult(requestCode, resultCode, data);
 if (requestCode == ACTION_REQUEST_CAMERA) {
     if (resultCode == RESULT_OK) {
       file = new File(data.getStringExtra(RESULT_IMAGE_PATH));
    }
  }
}
```

# Dependency

* Android Appcompact Library ``v27.1.1``
* Google Vision ``15.0.2``

## Credits

Desgin & Developed by : **[Jatin Sahgal](https://www.linkedin.com/in/jatinsahgal/)**
 (**[Linkedin](https://www.linkedin.com/in/jatinsahgal/)** & **[Website](http://androidcodelab.com/)** & **[Github](https://github.com/Lib-Jamun)**) 

## More Library under Jamun 

* **[Pickers](https://github.com/Lib-Jamun/Pickers.git)**
Pickers Library provide you a set of Pickers like Country, Language, Share and Intent Chooser.

* **[Country-Pickers](https://github.com/Lib-Jamun/Pickers.git)**
allow you to access Country picking functionality with great UI/UX design, and there are numberous of function which help you to modify picker as per your requirements. Library has been provided with four custom UI initate mode you can decide how the view of picker can be initate. You can also decide weather picker inheriate Single or Multi Selection property. Library consists of updated collection of country name, code and there flags. We are using APIs base structure to avoid increase in the size of apk due to flag Images. This module Maintain the database so that you don't need to call APIs again and again rather than you can choose when to refresh the Database and fetch new real time data.

* **[Language-Pickers](https://github.com/Lib-Jamun/Pickers.git)**
provides you read-made Language picker  which is easy to use and comes with great UI/UX, and there are numberous of function which help you to modify picker as per your requirements. Library has been provided with four custom UI initate mode you can decide how the view of picker can be initate. You can also decide weather picker inheriate Single or Multi Selection property.

* **[Calendar](https://github.com/Lib-Jamun/calendar.git)**
is a collection of Beautiful Activities which help others to make there Fully Custom Calendar View with Single and Multi Date Picker Functionality 

* **[Scanner](https://github.com/Lib-Jamun/scanner.git)**
is a collection of Beautiful Activity which help others to make there own Custom QR/Barcode Scanner. 

* **[Volley](https://github.com/Lib-Jamun/Volley.git)**
Library is a set of Custom Classes with UI components for network programming, integration and transaction handling in a better and standard way. This will help developers for making quality use of volley library. 

* **[UI](https://github.com/Lib-Jamun/ui.git)**
library is a set of UI Views, Custom Component and Collection of Helper Classes which help Developer for making quality Product. Such as Camera, Gallery, Number of Pickers, Calendar, Date Pickers, Dialogs and many more Heler UI and Backend Component.

* **[Gallery](https://github.com/Lib-Jamun/gallery.git)**
Library have splendid UI Components with Single and Multi files Selection Mode for android Developers to give there app a A Rich look With with custom picker functionality to cover up maximum media type like Audio, Files (Docs, Text etc) and Images.

* **[Elements](https://github.com/Lib-Jamun/elements.git)**
Library provide you a custom set of Android Elements that have custom views and properties like CircularImageView or CircularNetworkImageView and many more.

* **[Browser](https://github.com/Lib-Jamun/Browser.git)**
Library provide you two type Single Pager and Multi Pager In-APP Browser Functionality with Event Handling and Functions to Customize Views. It also provide you Copy to clipboard, Open in Browser and share link feature in-Bulit.

## License
    Copyright (c) 2018 Jatin Sahgal

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
  
  

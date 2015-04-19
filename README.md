# Google SpreadSheet Lib for Android
This Library helps to develop Android applications which can access Google SpreadSheets?. Though Google has mentioned that GData API supports SpreadSheet? API on Android, but this is not the case. There are multiple forums pointing this problem without any solution Problem#1 Problem#2.

It has been developed in Java with no platform dependency, so can be used in any Java based platform (Desktop, Android, J2ME and RIM).

Following are the supported features-

- Supports both List and Table feed
- Create/Delete SpreadSheet?
- Create/Delete WorkSheet?
- Insert/Update/Delete Worksheet data
- Conditional data retrieval (Structured Query support)
- Share SpreadSheet? with other users (Gmails IDs)
- 2 types of Authentications. Basic Authenticator and Android Authenticator. Basic Auth is suitable for non-Android applications where application need to prompt users for Gmail ID and Password. Whereas Android Auth uses Android's Account Manager concept and requires the relevant Gmail account should be registered under "Settings | Accounts and Synch".

The sample Android client application includes AndroidAuthenticator?.java which you can re-use.

Kindly note:
- This library doesn't support any persistent caching facility and if user plan for any caching, they need to develop separate logic.

- Prior to use the Sample Android application, make sure you have registered a valid Gmail Account under "Settings | Accounts and Synch".

- Android emulator strips out few XML feed prefix and thus need to add following line at the very beginning if you want to use this library in emulator-
````java
if("sdk".equals(Build.PRODUCT) || "google_sdk".equals(Build.PRODUCT))
    ParseFeed.doCustomizationForSDK();
````

Share your feedback, queries, comments on my blog, I'm listening :-)

#License
Copyright 2015 Prasanta Paul (http://prasanta-paul.blogspot.in/)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

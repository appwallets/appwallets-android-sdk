appwallets-android-sdk
======================

appwallets-android-sdk see (http://www.appwallets.com/) for more information.

##Installation
- copy `appwalletsAndroidSDK.jar` into your project libs


- copy Resource files to your project:
```javascript
res/drawable/*xml
res/drawable-xhdpi/*.png
layout/video_view.xml
layout/web_view.xml
values/dimens.xml
```

- add Permissions, Activities and anum in `AndroidManifest.xml`

```xml
	<uses-permission android:name="android.permission.INTERNET" />
	<uses-permission android:name="android.permission.WAKE_LOCK" />
	<uses-permission android:name="android.permission.READ_PHONE_STATE"/>
	
	<application ...
	
	       <activity
            android:name="com.wallets.appwalletsSDK.WebViewActivity"
            android:label="@string/title_activity_webview" >
        </activity>

        <activity
    android:name="com.wallets.appwalletsSDK.VideoViewActivity"
    android:label="@string/app_name"
    android:theme="@android:style/Theme.NoTitleBar.Fullscreen"
    android:screenOrientation="landscape" ></activity>
    
    <meta-data android:name="anum" android:value="100011" /> 
    
    
    </application>
    
```

Usages
--

```java
Intent myIntent = new Intent(MainActivity.this, WebViewActivity.class);
MainActivity.this.startActivity(myIntent);
			
			
```




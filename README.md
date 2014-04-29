appwallets-android-sdk
======================
copy appwalletsAndroidSDK.jar into your project libs

Usages
--

in AndroidManifest.xml

three Permission, two Activities and anum

```javascript
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



Resource files:

copy files to your project:


	res/drawable/*xml
	res/drawable-xhdpi/*.png
	layout/video_view.xml
	layout/web_view.xml
	values/dimens.xml


Call appWallet
--

```java
Intent myIntent = new Intent(MainActivity.this, WebViewActivity.class);
MainActivity.this.startActivity(myIntent);
			
			
```




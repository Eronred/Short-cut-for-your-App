**Open meta-data tag between activity tag,** 

```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.shortcutfprapp">

    <application
        android:allowBackup="true"
        android:icon="@drawable/profile_pic"
        android:label="@string/app_name"
        android:roundIcon="@drawable/profile_pic"
        android:supportsRtl="true"
        android:theme="@style/AppTheme">
        <activity android:name=".HomePage"
            >
        </activity>
        <activity android:name=".profile">

            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
            ### <meta-data android:name="android.app.shortcuts"
                android:resource="@xml/shortcuts" />
        </activity>
    </application>

</manifest>
```



> <meta-data android:name="android.app.shortcuts"
>                 android:resource="@xml/shortcuts" />

then create your xml as named here ""android:resource="@xml/shortcuts""".

now time for xml.

""keep it mind that this xml not will be in layout file.
### **>Write these code ;**
```
> <?xml version="1.0" encoding="utf-8"?>
> <shortcuts xmlns:android="http://schemas.android.com/apk/res/android">
>     <shortcut
>         android:shortcutId="home"
>         android:enabled="true"
>         android:icon="@drawable/home_icon"
>         android:shortcutShortLabel="@string/home"
>         android:shortcutLongLabel="@string/home">
>         <intent
>             android:action="android.intent.action.VIEW"
>             android:targetPackage="com.shortcutfprapp"
>             android:targetClass="com.shortcutfprapp.HomePage" />
> </shortcut>
> </shortcuts>
```

**give a name, icon, targetClass and more. You can create as much as you want!**

**android:targetPackage** must be your Package. 

Thats it! you will see this result; 
![google-app-shortcuts-4-840x560](https://user-images.githubusercontent.com/43992376/72807253-08cadf80-3c68-11ea-9a85-6cbba1fea3f2.jpg)

Do not forget to give star, fork and follow :) 

Follow me on [instagram ](https://www.instagram.com/eronred/)
for cooperation ; 

> **erencan_arica@hotmail.com**

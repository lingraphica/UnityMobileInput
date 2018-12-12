# UnityMobileInput
Unity Mobile Input Plugin for iOS and Android (Unity UI compatible)
You can use default InputField UI component on iOS and Android `without additional field` above keyboard

> It's deep refactor and bug fix of UnityNativeEdit (https://github.com/kmbang/UnityNativeEdit)

## Features
1. Native input field and keyboard on iOS and Android
2. Hiding additional mobile input box (Android)
3. Show "Done", "Clear" buttons (iOS)
4. Return button type: Default, Next, Done, Search 

## How to use
1. Copy the files into your existing unity project asset folder
2. Make empty Gameobject and attach ```Plugins``` to your new GameObject
3. Attach ```MobileInputField``` script to your Unity UI ```InputField``` object
4. For more options set ```ContentType``` to ```Custom``` to your ```InputField``` object
5. For `Android` make sure your `AndroidManifest.xml` has the following setting

```xml
<activity android:name="com.unity3d.player.UnityPlayerNativeActivity" android:label="@string/app_name">
            ...
            <meta-data android:name="unityplayer.ForwardNativeEventsToDalvik" android:value="true" />
            ...
</activity>
```
6. To prevent screen slide up on `Android` when keyboard show, add this option to your `AndroidManifest.xml`

```xml
<activity ...  android:windowSoftInputMode="adjustNothing">
            ...
</activity>
```

## Demo
Open Demo scene and build, to try how it works

## Example
[![UnityMobileInput Andorid demo](https://img.youtube.com/vi/181jrTj2Upg/0.jpg)](https://www.youtube.com/watch?v=181jrTj2Upg)

## Etc
> JSON library for C# is NiceJson (https://github.com/AngelQuirogaM/NiceJson)

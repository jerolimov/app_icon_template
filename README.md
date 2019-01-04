# Sketch template to create Android and iOS app icons

✅ Exports the **"standard" Android App Icons** as **rectangle and round icon**

✅ Exports the **"new" Android O [Adaptive App Icon Set](https://developer.android.com/guide/practices/ui_guidelines/icon_design_adaptive)** with its **separate background and foreground layer**

✅ Exports all required App Icons for iOS (iPhone and iPad)

✅ And finally, exports marketing icons for the AppStore and PlayStore.

<br/>

## Getting started

Clone or download ([zip-file](https://github.com/jerolimov/app_icon_template/archive/master.zip))
the complete repository, modify the Sketch file and export all assets.

The Sketch file uses Symbols and pre-defined Exports to make the usage streight forward.

## Android

To create all necessary icons you need to update the "Android Standard Icon" (first row, first icon)
as well as the Android Foreground and Android Background assets (second row, first and second icon).

Export than all icon sizes with File > Export... and copy the content of the `android/res` folder
into your Android project (into `the src/main/res` folder).

This includes your generated content as well as the mipmap-anydpi-v26 folder for
[Adaptive icons](https://developer.android.com/guide/practices/ui_guidelines/icon_design_adaptive).

You should also update your `AndroidManifest.xml` `application` tag and add or update this
two icon attributes:

```
    <application
        ....
        android:icon="@mipmap/ic_launcher"
        android:roundIcon="@mipmap/ic_launcher_round"
        ....
```

## iOS

Copy the icon asset bundle (the folder) `ios/AppIcon.appiconset` into your Xcode project
(into the folder with your project name/Images.xcassets).
This folder includes your generated content as well as the `Contents.json` file which
referes these icons (by their filename) already.

## Changelog

### 1.0

*   Initial version with support for Android Standard Icons,
    the Android Adaptive App Icon and iOS Icons.

## License

Created by Christoph Jerolimov. You can follow me on twitter: [@jerolimov](https://twitter.com/jerolimov)

Licensed unter [Creative Commons Attribution 4.0 International Public License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

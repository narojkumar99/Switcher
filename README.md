# Switcher

<img src="/art/preview.gif" alt="sample" title="sample" width="260" height="390" align="right" vspace="52" />

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Platform](https://img.shields.io/badge/platform-android-green.svg)](http://developer.android.com/index.html)
[![API](https://img.shields.io/badge/API-19%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=19)

Created this cool [switch animation](https://dribbble.com/shots/5429846-Switcher-XLIV) from [Oleg Frolov](https://dribbble.com/Volorf) as an android library. 

<a href="https://android.jlelse.eu/android-dynamic-custom-view-is-easy-433258cbb80f">
  <img alt="Read on Medium" src="/art/medium.png" width="196" height="80" hspace="15" />
</a>

USAGE
-----

Just add Switcher view in your layout XML and Switcher library in your project via Gradle:

```gradle
dependencies {
  implementation 'com.bitvale:switcher:1.0.0'
}
```

XML
-----

```xml
<com.bitvale.pacbutton.SwitcherX // or SwitcherC
    android:id="@+id/switcher"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    app:switcher_on_color="@color/on_color"
    app:switcher_off_color="@color/off_color"
    app:switcher_icon_color="@color/icon_color" />
```

You must use the following properties in your XML to change your Switcher.


##### Propertie:

* `android:checked`                 (boolean)   -> default  true
* `app:switcher_on_color`           (color)     -> default  #48ea8b
* `app:switcher_off_color`          (color)     -> default  #ff4651
* `app:switcher_icon_color`         (color)     -> default  white

Kotlin
-----

```kotlin
switcher.setOnCheckedChangeListener { checked ->
    if (checked) action()
}
```

LICENCE
-----

Switcher by [Alexander Kolpakov](https://play.google.com/store/apps/dev?id=7044571013168957413) is licensed under an [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).

# QR and Bar code reader with ZXing ("Zebra Crossing")

This project illustrates QR and Bar code reading in your Android project.

## Keypoint:

* Add ZXing dependency in 'build.gradle'

```gradle
  compile 'com.journeyapps:zxing-android-embedded:3.0.3@aar'
  compile 'com.google.zxing:core:3.2.0'
```

Ex. My 'build.gradle':

```gradle
apply plugin: 'com.android.application'

android {
    compileSdkVersion 22
    buildToolsVersion "22.0.1"

    defaultConfig {
        applicationId "com.example.heckyeahvince.qrscanner"
        minSdkVersion 15
        targetSdkVersion 22
        versionCode 1
        versionName "1.0"
    }
    buildTypes {
        release {
            minifyEnabled false
            proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.pro'
        }
    }
}

dependencies {
    compile fileTree(dir: 'libs', include: ['*.jar'])
    testCompile 'junit:junit:4.12'
    compile 'com.android.support:appcompat-v7:22.2.1'

  // added by mkc for ZXing
    compile 'com.journeyapps:zxing-android-embedded:3.0.3@aar'
    compile 'com.google.zxing:core:3.2.0'
}
```

Refer to the following project for more information:

* https://github.com/journeyapps/zxing-android-embedded 
 

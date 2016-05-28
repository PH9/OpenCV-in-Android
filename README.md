# Android with OpenCV

## Setup

#### 1. Download
OpenCV for Android 3.1 from [OpenCV Webs Site](http://opencv.org/platforms/android.html).

#### 2. Import module
To import OpenCV you have to import new module by `File > New > Import Module... > ` then locate your sdk folder for me is `~/Library/Android/OpenCV-android-sdk-3.1/sdk/java`

#### 3. Add dependency
Right click at your project folder in Android Studio ` > Open Modules Setting > 'Module' app > Dependencies 'tab' > + > Module Dependencies > select :libraries:OpenCV`.

#### 4. Copy .so
You need to create a JNI folder to `/app/src/main/jniLibs` and copy all folders with *.so files eg. arm64-v8a, armeabi, armeabi-v7a, mips, mips64, x86, x86_64 (choose CPU architecture you supported) into the jniLibs folder from the OpenCV SDK

* The folder you can find in `OpenCV SDK/sdk/native/libs/`
* You can delete all other non *.so files in the folders

#### 5. Sync your gradle
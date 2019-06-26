Building for Android

Pre-requisites

- Android Studio (3.4.1)
- CMake (install using SDK manager in Android Studio)
- Android NDK r20
- Ninja (brew install ninja)
- Bontouch OpenCV repo 

JAVA_HOME="/Applications/Android Studio.app//Contents/jre/jdk/Contents/Home/jre/"
PATH=$JAVA_HOME/bin:$PATH
ANDROID_NDK=/Users/roland/Desktop/android-ndk-r20
ANDROID_SDK=/Users/roland/Library/Android/sdk

mkdir build && cd build
../opencv.git/platforms/android/build_sdk.py --config ../opencv.git/bontouch/android/ndk-20.config.py --ndk_path $ANDROID_NDK --sdk_path $ANDROID_SDK  . ../opencv.git


# apk-devtool
apk development on the command line (no gradle or ant)

# description
A helper for developing android app.

Currently support:
- apk building

Works on termux!

How to use (quick start):
```
cd ~
pkg install openjdk-17 aapt2 d8 apksigner zip git curl android-tools
git clone https://github.com/wmartinmimi/apk-devtool
./apk-devtool/android-32-download
ln -s ~/apk-devtool/apkdev $PREFIX/bin/apkdev
cd <android-project-root>
apkdev
```

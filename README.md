# apk-devtool
apk development on the command line (no gradle or ant)

## description
A helper for developing android app.

## features
Currently support:
- apk building

If you want to change some variables,
you have to modify apkdev for now.
Sorry!

Works on termux!

## How to use (quick start)
```
cd ~
pkg install openjdk-17 aapt2 d8 apksigner zip git curl android-tools
git clone https://github.com/wmartinmimi/apk-devtool
cd apk-devtool
./android-32-download
ln -s ~/apk-devtool/apkdev $PREFIX/bin/apkdev
cd <android-project-root>
apkdev
```
build/output.signed.apk will be produced,
you can open it with
```
termux-open build/output.signed.apk
```
but requires ```allow-external-apps = true``` in ~/.termux/termux.properties

## requests / issues

If someone request a feature, I would try my best to add it.

We welcome any issues or contributions!

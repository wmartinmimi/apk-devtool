# Apk-Devtool

apk development on the command line (no gradle or ant)

## Description

A helper for developing android app.

## Features

Currently supporting:

- apk building
- project creation
- both java and kotlin code

If you want to change some variables,
you can modify config file in apk-devtool directory.

Works on termux!

## How to use (quick start)

```bash
cd ~
pkg install git
git clone https://github.com/wmartinmimi/apk-devtool
cd apk-devtool
./quick-setup
cd <android-project-root>
apkdev build
```

build/output.signed.apk will be produced,
you can open it with

```bash
termux-open build/output.signed.apk
```

but requires ```allow-external-apps = true``` in ~/.termux/termux.properties

you can create a new project with apkdev,
just do

```bash
apkdev new
```

it will prompt for basic details,
and create a hello world project at ```<project-name>/```.

the created project is ready to run on default.

for different builds, you can do

```bash
apkdev build release
```

or

```bash
apkdev build debug
```

to download maven jars, do

```bash
apkdev m d <groupid>:<id>:<version> <url>
```

examples:

```bash
apkdev m d androidx.core:core:1.9.0
```

```bash
apkdev m d org.mozilla.components:support-base:105.0.6 https://maven.mozilla.org/maven2
```

if you need the help manual, do

```bash
apkdev help
```

## requests / issues

If you request a feature, I would try my best to add it.

We welcome any issues or contributions!

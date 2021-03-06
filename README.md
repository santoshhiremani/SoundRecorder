# Easy Sound Recorder 2
[![API](https://img.shields.io/badge/API-16%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=16) [![Build Status](https://travis-ci.com/naXa777/SoundRecorder.svg?branch=master&style=flat)](https://travis-ci.com/naXa777/SoundRecorder) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/1b4c1e2546784537b6bef070769c34bb)](https://www.codacy.com/app/naXa777/SoundRecorder?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=naXa777/SoundRecorder&amp;utm_campaign=Badge_Grade)

A simple sound recording Android app implementing <a href="https://material.io/">Material Design</a>.

![Icon](/app/src/main/res/mipmap-hdpi/ic_launcher.png) [![Android app on Google Play](https://d.android.com/images/brand/en_app_rgb_wo_60.png)](https://play.google.com/store/apps/details?id=by.naxa.soundrecorder)

## Contributing

Contributors are more than welcome. How can you contribute?

### Report bugs

We want our app to be as stable as possible thus your bug reports are immensely valuable. File [GitHub Issues](https://github.com/naXa777/SoundRecorder/issues) for anything that is unexpectedly broken.

* App version
* Device model
* Android version
* Steps to reproduce the bug
* Expected behavior
* Actual behavior (a screenshot and/or log file may be helpful)

### Contribute Code [![Open Source Helpers](https://www.codetriage.com/naxa777/soundrecorder/badges/users.svg)](https://www.codetriage.com/naxa777/soundrecorder)

We have labeled tasks you can help with as [![GitHub issues by-label](https://img.shields.io/github/issues/naXa777/SoundRecorder/help%20wanted.svg)](https://github.com/naXa777/SoundRecorder/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) and [![GitHub issues by-label](https://img.shields.io/github/issues/naXa777/SoundRecorder/good%20first%20issue.svg)](https://github.com/naXa777/SoundRecorder/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22). Just pick up an issue that you're interested in and start coding. If you have a great idea you really want to implement, start by logging an issue for us. We'll let you know if it fits with our product direction and then you can start development. When you're ready open a Pull Request with a description of your changes.

A quick note: See Chris Beams' guide to writing good commit messages - [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/).

### Translate

You don't have to be a programmer if you want to translate this application in your own language or improve existing translations.
You can translate SoundRecorder using [POEditor](https://poeditor.com/join/project/IuPsne4VcJ) - a collaborative translation platform.

[![POEditor](https://poeditor.com/public/images/logo_small.png)](https://poeditor.com/join/project/IuPsne4VcJ)

### Automate Testing

Testing is imperative to the health of the project. There's a configured CI pipeline ([Travis CI](https://travis-ci.com/naXa777/SoundRecorder)) intended for running unit tests and instrumented tests on every commit to the repository, but unfortunately, there're very few tests at the moment.

Please follow standard guidelines if you want to contribute a test:

1. Android Developers - [Test apps on Android](https://d.android.com/training/testing/)
2. Android Studio - [Test your app](https://d.android.com/studio/test/)
3. GitHub - [Android testing samples](https://github.com/googlesamples/android-testing)

## Screenshots

![Imgur](https://i.imgur.com/wxCXesJl.png) ![Imgur](https://i.imgur.com/86sehcjl.png)
![Imgur](https://i.imgur.com/p9Pn9Qgl.png) ![Imgur](https://i.imgur.com/LthDOjHl.png)
![Imgur](https://i.imgur.com/KCODDi8l.png) ![Imgur](https://i.imgur.com/rxeQUDIl.png)
![Imgur](https://i.imgur.com/U6w7dnXl.png) ![Imgur](https://i.imgur.com/ZGRnroNl.png)

## Building

If you want to run the app locally, do the following:

1. Download or clone the repository
2. If you don't have a Fabric account -> Sign up at fabric.io
3. Declare environment variables of which the name starts with `ORG_GRADLE_PROJECT_` followed by the property name (include your own Fabric `apiKey` and `apiSecret`).
     `export ORG_GRADLE_PROJECT_soundrecorderCrashlyticsApiSecret=0cf7c9df6d057e7bb62b1427ab364e8115a75fcf7430873b6274bb094d1a8adb`   
     `export ORG_GRADLE_PROJECT_soundrecorderCrashlyticsApiKey=cc238b2a4866c96030`
   Then `fabric.properties` file will be created automatically by Gradle on the first build. Do not commit this file to a version control, keep it secret.
4. Import the project in your IDE (we use Gradle + Android Studio to build)
5. You should now be able to build and run the app.

See [Crashlytics Kit Setup Demo](https://github.com/plastiv/CrashlyticsDemo) if you need more help.

## Dev environment

- [Android Studio](https://d.android.com/studio/preview/) 3.3 (Canary) is used for development
- [Gradle](https://gradle.org/install/) 4.10 is used to build the project
- [Android SDK 9.0](https://d.android.com/studio/releases/platforms#9.0) (Pie), API level 28
- Java 1.6

## Permissions needed for the app are:

- record audio
- write to external storage (to store recordings)
- read from external storage (to playback recordings)
- internet access (for stats collection)

Since February 2017 Google enforces a strict privacy policy requirement for apps using sensitive permissions (the RECORD_AUDIO permission). See [Privacy Policy](https://soundrecorder.bitbucket.io/privacy_policy.html) of Easy Sound Recorder 2.

## Credits / Libraries used:

- [Java MP4 Parser](https://github.com/sannies/mp4parser)
- [Circular Progress Bar](https://github.com/yuriy-budiyev/circular-progress-bar)
- [Material Components for Android](https://github.com/material-components/material-components-android)

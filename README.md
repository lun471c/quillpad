[![Gitter](https://badges.gitter.im/quillpad/community.svg)](https://gitter.im/quillpad/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
[![Android Build Release](https://github.com/quillpad/quillpad/actions/workflows/android.yml/badge.svg?branch=master)](https://github.com/quillpad/quillpad/actions/workflows/android.yml)
# Quillpad
Quillpad is fully free and open-source. It will never show you ads, ask you for unnecessary permissions or upload your notes anywhere without you knowing.

Take beautiful markdown notes whenever you feel inspired. Place them in notebooks and tag them accordingly. Stay organized by making task lists, set reminders and keep everything in one place by attaching related files.

### Matrix
Join the conversation at [Matrix](https://matrix.to/#/#quillpad_community:gitter.im) or [Gitter](https://gitter.im/quillpad/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

### Fork Info
Quillpad is a fork of an original app called [Quillnote](https://github.com/msoultanidis/quillnote). The development stopped on the original app and PR backlogs were not cleared up. The community showed much interest in the app for continued development and so this fork was created. https://github.com/msoultanidis/quillnote/issues/177 https://github.com/msoultanidis/quillnote/issues/209

<img src="fastlane/metadata/android/en-US/images/phoneScreenshots/1.png" width="256"/><img src="fastlane/metadata/android/en-US/images/phoneScreenshots/2.png" width="256"/><img src="fastlane/metadata/android/en-US/images/phoneScreenshots/4.png" width="256"/>


<a href="https://f-droid.org/packages/io.github.quillpad">
    <img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png"
    alt="Get it on F-Droid"
    height="80">
</a>
<a href='https://play.google.com/store/apps/details?id=io.github.quillpad'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png' height="80"/></a>



## Features
With Quillpad, you can:

- Take notes with Markdown support
- Make task lists
- Pin your favorite notes to the top
- Hide notes you do not want others to see
- Set reminders for events you do not want to miss
- Add voice recordings and other file attachments
- Group related notes in notebooks
- Add tags to notes
- Archive notes you want out of your way
- Search through notes
- Sync with Nextcloud (experimental)
- Backup your notes to a zip file which you can restore at a later time
- Toggle between Light and Dark mode
- Choose between multiple color schemes

## Migration
Backups from [Notally](https://github.com/OmGodse/Notally) can be converted into Quillpad compatible backups using this [python script](https://gist.github.com/nWestie/224d14a6efd00661b5c93040c7511816)

## Roadmap
The major features that are currently planned for this app are listed below in a series of milestones. In additional to these major features, there will be bug fixes and other enhancements will be added as we go. 

### Milestone 1.5 (General cloud syncing)
- Store the notes as markdown files in the device. 
- If the folder chosen is under a cloud storage provider, Android will sync the markdown files with the respective cloud. For e.g. Google Drive, Dropbox and even Nextcloud. Syncing this way to the cloud does not deal with the Nextcloud API.
- This will be the easiest way for users to sync the notes without having to self-host a NextCloud instance.
- Update to the latest version of Android API and Dependency Libraries.

### Milestone 1.6 (Jetpack Compose)
- Introduce Compose and Kotlin multiplatform. The main app views like the list of notes, edit view and the todo list view will be migrated to Compose. 

### Milestone 1.7 (Desktop App)
- Introduce desktop app. With the main views available in compose, try making a desktop app with help of Compose for desktop.
  
### Milestone 1.8 (iOS App)
- Try an iOS version since the kotlin multiplatform code does the heavy lifting of notes management and syncing. Leverage the same storage API equivalent in iOS.

### Milestone 2.0 (Encryption)
- The primary motive to have encryption is not for security. That's secondary
- Now we have the ability to sync notes using cloud providers like Google Drive and Dropbox. The cloud providers _may_ to go through the notes and _may_ index them and _may_ profile the user. This is the primary reason for the encryption feature. Which means, the notes won't be staying as markdown files, and cannot be edited by other text editors. 
- Encryption will be optional. The user can switch between having the notes encrypted vs stored them as plain markdown files.
- The main focus  

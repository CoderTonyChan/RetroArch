[![Build Status](https://travis-ci.org/libretro/RetroArch.svg?branch=master)](https://travis-ci.org/libretro/RetroArch)
[![Coverity Scan Build Status](https://scan.coverity.com/projects/8936/badge.svg)](https://scan.coverity.com/projects/retroarch)

# RetroArch

## iOS Compilation / Development Guide
https://docs.libretro.com/development/retroarch/compilation/ios/

### Code Signing the Cores

Note that you must code sign the dylib cores in order for you to use them.

In iOS 9 and above

Starting from iOS 9, the cores must be packaged as part of the application, even if they are code-signed. This was an additional security measure introduced in iOS 9. Fortunately, the code signing is handled as part of the Xcode build/archive process, so all you need to do is place your compiled .dylib cores in the pkg/apple/iOS/modules folder. Running the application via Xcode or archiving the application for an adhoc distribution will codesign the cores as long as they are placed in the aforementioned pkg/apple/iOS/modules folder.


### Building RetroArch

FOR IOS 10 AND UP

Open Xcode.
Open the following project file pkg/apple/RetroArch_iOS10.xcodeproj
In the Navigator Pane on the left, select the Retroarch_iOS10 project
In the Project and Targets list on the left side, choose the RetroArchiOS10 target. Select the Target (the one with the RetroArch icon), not the project.
In the "General" tab, change the "Team" under Signing to be your developer name.
Set the active scheme to RetroArchiOS10, and select your connected iOS device as the device.
Run (⌘-R)


### Core
[iOS Jailbroken] — RetroArch 1.8.1 and other emulators (Cydia & Sileo)
https://forums.libretro.com/t/ios-jailbroken-retroarch-1-8-1-and-other-emulators-cydia-sileo/24668

http://johan.margueritte.free.fr/buildbot/ios-arm64
http://johan.margueritte.free.fr/buildbot/tvos-arm64/

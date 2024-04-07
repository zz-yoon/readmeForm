# readmeForm

Created a common README File - Vercompany

# Project Name

- Project Name

# Table Of Contents(TOC)

- [BasicSettings](#BasicSettings)
- [ProjectSettings](#ProjectSettings)
- [Usage](#Usage)
- [ReferenceDocument](#ReferenceDocument)

# Basic Settings

1. git settings
2. android studio settings
3. ios xcode settings

# Project Settings

1.  flutter sdk 다운로드
    <https://docs.flutter.dev/get-started/install/windows>
2.  압축 풀고 `C:\flutter` 위치에 폴더를 만든 후 해당 폴더에 압축 푼 파일을 푼다
3.  환경변수 설정
    시스템 환경 변수 편집 > 고급설정 > 환경변수 > 시스템변수 > path에 `C:\flutter\bin`추가

4.  android studio settings

- file > settings > plugins 에서 flutter, dart install
- flutter sdk 위치 설정 : file > new > new flutter project flutter sdk
  `C:\flutter platforms: aos.ios.web`

## Git Settings

1. file > settings > Version Control > Git(\*git이 설치되어 있는지 test 버튼을 눌러 test)
2. file > settings > Version Control > Github - Log in with Token 깃 계정 연결
3. Repository와 프로젝트 연동
   VCS > Enavle Version Control Integration
4. git > Manager Remotes > git clone url 등록

## Project Folder Structure

1. 폴더 구조를 작성해주세요.

- vscode가 아닌 다른 ide 사용할 경우 Project Tree Genertator
  <https://woochanleee.github.io/>
- vscode project-tree extension 사용 : `ctrl + shipt + p` 후 project-tree 검색시 readme에 알아서 추가됨

```
todaymeal2.0
├─ .git
│  ├─ config
│  ├─ description
│  ├─ HEAD
│  ├─ hooks
│  │  ├─ applypatch-msg.sample
│  │  ├─ commit-msg.sample
│  │  ├─ fsmonitor-watchman.sample
│  │  ├─ post-update.sample
│  │  ├─ pre-applypatch.sample
│  │  ├─ pre-commit.sample
│  │  ├─ pre-merge-commit.sample
│  │  ├─ pre-push.sample
│  │  ├─ pre-rebase.sample
│  │  ├─ pre-receive.sample
│  │  ├─ prepare-commit-msg.sample
│  │  └─ update.sample
│  ├─ index
│  ├─ info
│  │  └─ exclude
│  ├─ logs
│  │  ├─ HEAD
│  │  └─ refs
│  │     ├─ heads
│  │     │  └─ master
│  │     └─ remotes
│  │        └─ origin
│  │           └─ HEAD
│  ├─ objects
│  │  ├─ info
│  │  └─ pack
│  │     ├─ pack-e8e5960507564c2e8521905d01c1d4d3c4dd657e.idx
│  │     └─ pack-e8e5960507564c2e8521905d01c1d4d3c4dd657e.pack
│  ├─ packed-refs
│  └─ refs
│     ├─ heads
│     │  └─ master
│     ├─ remotes
│     │  └─ origin
│     │     └─ HEAD
│     └─ tags
├─ .gitignore
├─ .metadata
├─ analysis_options.yaml
├─ android
│  ├─ .gitignore
│  ├─ .gradle
│  │  ├─ 7.5
│  │  │  ├─ checksums
│  │  │  │  └─ checksums.lock
│  │  │  ├─ dependencies-accessors
│  │  │  │  ├─ dependencies-accessors.lock
│  │  │  │  └─ gc.properties
│  │  │  ├─ executionHistory
│  │  │  │  ├─ executionHistory.bin
│  │  │  │  └─ executionHistory.lock
│  │  │  ├─ fileChanges
│  │  │  │  └─ last-build.bin
│  │  │  ├─ fileHashes
│  │  │  │  ├─ fileHashes.bin
│  │  │  │  ├─ fileHashes.lock
│  │  │  │  └─ resourceHashesCache.bin
│  │  │  ├─ gc.properties
│  │  │  └─ vcsMetadata
│  │  ├─ buildOutputCleanup
│  │  │  ├─ buildOutputCleanup.lock
│  │  │  ├─ cache.properties
│  │  │  └─ outputFiles.bin
│  │  ├─ file-system.probe
│  │  ├─ kotlin
│  │  │  ├─ errors
│  │  │  └─ sessions
│  │  └─ vcs-1
│  │     └─ gc.properties
│  ├─ app
│  │  ├─ build.gradle
│  │  ├─ google-services.json
│  │  └─ src
│  │     ├─ debug
│  │     │  └─ AndroidManifest.xml
│  │     ├─ main
│  │     │  ├─ AndroidManifest.xml
│  │     │  ├─ java
│  │     │  │  └─ io
│  │     │  │     └─ flutter
│  │     │  │        └─ plugins
│  │     │  │           └─ GeneratedPluginRegistrant.java
│  │     │  ├─ kotlin
│  │     │  │  └─ com
│  │     │  │     └─ example
│  │     │  │        └─ todaymeal
│  │     │  │           └─ MainActivity.kt
│  │     │  └─ res
│  │     │     ├─ drawable
│  │     │     │  ├─ background.png
│  │     │     │  └─ launch_background.xml
│  │     │     ├─ drawable-hdpi
│  │     │     │  ├─ android12splash.png
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-mdpi
│  │     │     │  ├─ android12splash.png
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-night-hdpi
│  │     │     │  └─ android12splash.png
│  │     │     ├─ drawable-night-mdpi
│  │     │     │  └─ android12splash.png
│  │     │     ├─ drawable-night-xhdpi
│  │     │     │  └─ android12splash.png
│  │     │     ├─ drawable-night-xxhdpi
│  │     │     │  └─ android12splash.png
│  │     │     ├─ drawable-night-xxxhdpi
│  │     │     │  └─ android12splash.png
│  │     │     ├─ drawable-v21
│  │     │     │  ├─ background.png
│  │     │     │  └─ launch_background.xml
│  │     │     ├─ drawable-xhdpi
│  │     │     │  ├─ android12splash.png
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-xxhdpi
│  │     │     │  ├─ android12splash.png
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-xxxhdpi
│  │     │     │  ├─ android12splash.png
│  │     │     │  └─ splash.png
│  │     │     ├─ mipmap-hdpi
│  │     │     │  └─ ic_launcher.png
│  │     │     ├─ mipmap-mdpi
│  │     │     │  └─ ic_launcher.png
│  │     │     ├─ mipmap-xhdpi
│  │     │     │  └─ ic_launcher.png
│  │     │     ├─ mipmap-xxhdpi
│  │     │     │  └─ ic_launcher.png
│  │     │     ├─ mipmap-xxxhdpi
│  │     │     │  └─ ic_launcher.png
│  │     │     ├─ values
│  │     │     │  ├─ colors.xml
│  │     │     │  └─ styles.xml
│  │     │     ├─ values-night
│  │     │     │  └─ styles.xml
│  │     │     ├─ values-night-v31
│  │     │     │  └─ styles.xml
│  │     │     └─ values-v31
│  │     │        └─ styles.xml
│  │     └─ profile
│  │        └─ AndroidManifest.xml
│  ├─ build.gradle
│  ├─ gradle
│  │  └─ wrapper
│  │     ├─ gradle-wrapper.jar
│  │     └─ gradle-wrapper.properties
│  ├─ gradle.properties
│  ├─ gradlew
│  ├─ gradlew.bat
│  ├─ local.properties
│  └─ settings.gradle
├─ assets
│  ├─ icons
│  │  ├─ home.svg
│  │  └─ home_active.svg
│  └─ image
│     ├─ splash.png
│     └─ splash.svg
├─ flutter_native_splash.yaml
├─ ios
│  ├─ .gitignore
│  ├─ Flutter
│  │  ├─ AppFrameworkInfo.plist
│  │  ├─ Debug.xcconfig
│  │  ├─ flutter_export_environment.sh
│  │  ├─ Generated.xcconfig
│  │  └─ Release.xcconfig
│  ├─ Runner
│  │  ├─ AppDelegate.swift
│  │  ├─ Assets.xcassets
│  │  │  ├─ AppIcon.appiconset
│  │  │  │  ├─ Contents.json
│  │  │  │  ├─ Icon-App-1024x1024@1x.png
│  │  │  │  ├─ Icon-App-20x20@1x.png
│  │  │  │  ├─ Icon-App-20x20@2x.png
│  │  │  │  ├─ Icon-App-20x20@3x.png
│  │  │  │  ├─ Icon-App-29x29@1x.png
│  │  │  │  ├─ Icon-App-29x29@2x.png
│  │  │  │  ├─ Icon-App-29x29@3x.png
│  │  │  │  ├─ Icon-App-40x40@1x.png
│  │  │  │  ├─ Icon-App-40x40@2x.png
│  │  │  │  ├─ Icon-App-40x40@3x.png
│  │  │  │  ├─ Icon-App-60x60@2x.png
│  │  │  │  ├─ Icon-App-60x60@3x.png
│  │  │  │  ├─ Icon-App-76x76@1x.png
│  │  │  │  ├─ Icon-App-76x76@2x.png
│  │  │  │  └─ Icon-App-83.5x83.5@2x.png
│  │  │  ├─ LaunchBackground.imageset
│  │  │  │  ├─ background.png
│  │  │  │  └─ Contents.json
│  │  │  └─ LaunchImage.imageset
│  │  │     ├─ Contents.json
│  │  │     ├─ LaunchImage.png
│  │  │     ├─ LaunchImage@2x.png
│  │  │     ├─ LaunchImage@3x.png
│  │  │     └─ README.md
│  │  ├─ Base.lproj
│  │  │  ├─ LaunchScreen.storyboard
│  │  │  └─ Main.storyboard
│  │  ├─ GeneratedPluginRegistrant.h
│  │  ├─ GeneratedPluginRegistrant.m
│  │  ├─ Info.plist
│  │  └─ Runner-Bridging-Header.h
│  ├─ Runner.xcodeproj
│  │  ├─ project.pbxproj
│  │  ├─ project.xcworkspace
│  │  │  ├─ contents.xcworkspacedata
│  │  │  └─ xcshareddata
│  │  │     ├─ IDEWorkspaceChecks.plist
│  │  │     └─ WorkspaceSettings.xcsettings
│  │  └─ xcshareddata
│  │     └─ xcschemes
│  │        └─ Runner.xcscheme
│  ├─ Runner.xcworkspace
│  │  ├─ contents.xcworkspacedata
│  │  └─ xcshareddata
│  │     ├─ IDEWorkspaceChecks.plist
│  │     └─ WorkspaceSettings.xcsettings
│  └─ RunnerTests
│     └─ RunnerTests.swift
├─ lib
│  ├─ constants
│  │  ├─ gaps.dart
│  │  └─ sizes.dart
│  ├─ main.dart
│  ├─ models
│  │  ├─ app_state_model.dart
│  │  ├─ product_model.dart
│  │  ├─ recipe_detail_model.dart
│  │  └─ recipe_model.dart
│  ├─ screens
│  │  ├─ home
│  │  │  └─ home_screen.dart
│  │  ├─ main_navigation
│  │  │  └─ main_navigation_screen.dart
│  │  ├─ muckshot
│  │  │  └─ muckshot_screen.dart
│  │  ├─ nanum
│  │  │  └─ nanum_screen.dart
│  │  ├─ Recipe
│  │  │  ├─ recipe_detail_screen.dart
│  │  │  └─ recipe_screen.dart
│  │  ├─ store
│  │  │  └─ store_screen.dart
│  │  └─ test
│  │     └─ test_screen.dart
│  ├─ services
│  │  ├─ product_api.dart
│  │  └─ recipe_api.dart
│  └─ widgets
│     ├─ media_model.dart
│     ├─ navi_item.dart
│     └─ tab_content.dart
├─ pubspec.lock
├─ pubspec.yaml
├─ README.md
├─ test
│  └─ widget_test.dart
└─ web
   ├─ favicon.png
   ├─ firebase-messaging-sw.js
   ├─ icons
   │  ├─ Icon-192.png
   │  ├─ Icon-512.png
   │  ├─ Icon-maskable-192.png
   │  └─ Icon-maskable-512.png
   ├─ index.html
   └─ manifest.json

```

## Project Naming Convention

1. 네이밍 컨벤션을 작성해주세요.

## Project .env

1. env파일 위치
2. .env 내용 (\*추가될때마다 업데이트)

# Usage

1. 어떻게 프로젝트 실행이 가능한가 작성

# Reference Document

1. 추가 참고문서 작성

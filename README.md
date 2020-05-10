# 설치

## 윈도우

### amd ryzen CPU 사용시 필수 (intel haxm 가속화 - Android studio 내장 AVD 사용시에만)

1. VT(SVM) 사용 
- https://lorans.tistory.com/7

2. Hyper-v enable
관리자 권한 powershell

- Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All

### app:installDebug , app:transformClassesWithDexBuilderForDebug
cd android

.\gradlew clean (start gradlew clean )

- SDK Tools NDK install

### virtual divice
- 지니모션

### 환경변수 등록

- ANDROID_HOME= C:\Users\[사용자 이름]\AppData\Local\Android\Sdk
- PATH = C:\Users\[사용자 이름]\AppData\Local\Android\Sdk\platform-tools
### 에러 고친뒤

- C:\Users\[사용자 이름]\.android\cache 삭제

### 확인할것
- adb 연결된거 없으면 에러

### 파이썬 버전
- 무조건 2만 가능


## MAC OSX
```bash
brew install node
brew install watchman
sudo gem install cocoapods
Xcode 설치
brew tap AdoptOpenJDK/openjdk
brew cask install adoptopenjdk8
https://developer.android.com/studio 안드로이드 스튜디오 설치
```
- https://velog.io/@shortdary/%EB%A6%AC%EC%95%A1%ED%8A%B8-%EB%84%A4%EC%9D%B4%ED%8B%B0%EB%B8%8C-%EA%B0%9C%EB%B0%9C%ED%99%98%EA%B2%BD-%EC%84%B8%ED%8C%85-Mac-RN-CLI-QuickStart
- https://dev-yakuza.github.io/ko/react-native/install-on-mac/

### 환경 변수 
```bash
export ANDROID_HOME=자신의 안드로이드SDK 위치/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/tools/bin
export PATH=$PATH:$ANDROID_HOME/platform-tools

source $HOME/.bash_profile
echo $PATH
```
### 에러
1. Please accept all necessary Android SDK licenses using Android SDK Manager
```
1> Navigate to Android studio:- ~/Library/Android/sdk/tools/bin

2> Run this command:- sdkmanager --licenses
```

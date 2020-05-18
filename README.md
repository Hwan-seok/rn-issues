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

#### Android Virtual Devices
1. bridge configuration isn’t available
`adb -s <device name> tcp:8081 tcp:8081`

### 디바이스 연결
- USB : https://aboutreact.com/how-to-run-react-native-app-on-real-device-android/
- WIFI : https://aboutreact.com/run-app-on-real-device-using-wi-fi/ 

### 패키지명 변경
1. /android/app/src/main/AndroidManifest.xml

2. 폴더구조 변경하기

3. app/build.gradle

4. /android/app/src/main/ 아래 있는 java 파일입니다.
https://romeoh.tistory.com/entry/React-Native-%ED%8C%A8%ED%82%A4%EC%A7%80%EB%AA%85-%EB%B2%88%EB%93%A4%EB%AA%85-%EB%B3%80%EA%B2%BD%ED%95%98%EA%B8%B0-Package-Bundle-Android-iOS

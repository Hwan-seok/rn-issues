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

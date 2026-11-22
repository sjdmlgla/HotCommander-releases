# HotCommander 배포 저장소

C17 / Win32로 만든 Windows 두 패널 파일 관리자 **HotCommander**의 설치·업데이트 파일만 올리는 저장소입니다. 소스 코드는 공개하지 않습니다.

## 설치

1. [최신 릴리스](https://github.com/sjdmlgla/HotCommander-releases/releases/latest)에서 `Setup_HotCommander.exe`를 내려받습니다.
2. 실행하면 `C:\HotUtility\HotCommander`(바꿀 수 있음)에 설치하고, 이미 설치되어 있으면 새 버전으로 업데이트합니다. 관리자 권한은 필요하지 않습니다.
3. 제거는 Windows 설정 → 앱 → 설치된 앱 → HotCommander에서 합니다.

## 자동 업데이트

Setup으로 설치한 HotCommander는 시작할 때 하루 한 번 이 저장소의 최신 릴리스를 확인합니다. 새 버전이 있으면 알려 주고, [지금 업데이트]를 누르면 설치 파일을 내려받아 함께 올린 `Setup_HotCommander.exe.sha256` 검증값과 같을 때만 실행해 새 버전으로 바꿉니다. 도움말 → 업데이트 확인에서 직접 확인할 수도 있고, 옵션에서 자동 확인을 끌 수 있습니다.

## 검증값 확인

```
certutil -hashfile Setup_HotCommander.exe SHA256
```

결과가 릴리스의 `Setup_HotCommander.exe.sha256` 내용과 같아야 합니다.
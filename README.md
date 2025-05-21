# Vue.js-Study
Vue.js 공부

# Vue VSCode 터미널에서 설정시 스크립트 실행 오류 해결
1. Windows PowerShell 앱을 검새하여 관리자로 실행합니다.

2. 현재 권한상태를 확인합니다.  > get-ExecutionPolicy
Restricted면 스크립트를 실행 할 수 없음

3. 권한 상태를 "RemoteSigned"으로 변경합니다. > Set-ExecutionPolicy RemoteSigned > Y

4. VSCode 실행

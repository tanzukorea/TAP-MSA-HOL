## 실습 환경 체크
다음의 파일들이 설치되어 있는지 확인합니다.
* SSH 도구: Putty
* Tanzu CLI
* kubectl CLI
* VSCode IDE 및 TAP용 Plugin

***참고 : 본 Lab은 Windows OS 기준으로 진행됩니다.**

### 0. 파일 준비
https://drive.google.com/drive/folders/1-z8_jvzTQd6FrGiGkFO5nyKsNA54l1ku 에서 필요한 파일들을 다운받습니다.

### 1. Putty 설치
**0. 파일 준비** 에서 다운받은 putty를 클릭해 실행을 확인합니다.

### 2. Tanzu CLI 설치
C드라이브 아래에 tanzu 디렉토리를 생성하고, 다운로드한 Tanzu tar 파일 **(tanzu-framework-windows-amd64)** 을 이곳으로 이동시켜 압축을 해제합니다.  <br/>


Program Files\tanzu 디렉토리에서 실행 파일을 다음 위치로 이동하고 이름을 바꿉니다.

기존 : Program Files\tanzu\cli\core\v0.11.2\tanzu-core-windows_amd64.exe
<br/> 에서 <br>
tar -xvf tanzu-framework-darwin-amd64.tar -C $HOME/tanzu


Program Files 디렉토리에서 tanzu 디렉토리를 마우스 오른쪽 버튼으로 클릭하고 속성 > 보안을 선택합니다.

사용자 계정에 모든 권한이 있는지 확인하십시오.

Windows 검색을 사용하여 env를 검색합니다.

시스템 환경 변수 편집을 선택하고 환경 변수를 클릭합니다.

시스템 변수에서 경로 행을 선택하고 편집을 클릭하십시오.

새로 만들기를 클릭하여 새 행을 추가하고 tanzu.exe의 경로를 입력합니다.

환경 변수 TANZU_CLI_NO_INIT를 true로 설정하십시오.

Program Files\tanzu 디렉토리의 터미널에서 다음을 실행하여 설치를 확인합니다.

탄즈 버전
예상되는 결과:

버전: v0.11.2
...
Tanzu CLI 플러그인 설치/업데이트 진행

### 3. kubectl CLI 설치
**0. 파일 준비** 에서 받은 Kubectl을 Windows 환경 변수에 추가합니다.

![](../images/env_set_00.png)
C 드라이브 아래에 Kube라는 디렉토리를 생성하고, 다운받은 Kubectl 파일을 이곳으로 이동시킵니다. <br/>

![](../images/env_set_01.png)
Windows 키를 눌러 Advanced System Setting을 검색합니다.<br/>

![](../images/env_set_02.png)
창 맨 아래의 Environment Variables를 클릭합니다.<br/>

![](../images/env_set_03.png)
Path를 선택 후 Edit을 클릭합니다.<br/>

![](../images/env_set_04.png)
NEW 클릭 -> C:\Kube를 입력하고, OK 버튼을 클릭합니다. 처음에 열었던 Advanced System Setting 창이 닫힐 때 까지 OK를 클릭합니다.<br/>

![](../images/env_set_05.png)
cmd를 열어 kubectl version을 입력하고, 아래와 같이 버전 정보가 뜨는지 확인합니다.

<br/>
### 4. VSCode IDE 및 TAP용 Plugin 설치

#### 1) VSCode IDE 설치


#### 2) TAP용 Plugin 설치


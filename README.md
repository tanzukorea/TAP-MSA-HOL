# TAP-HOL

 (VMware Tanzu Application Platform Hands-On-Lab)
 ![](images/tanzu_hol_header_logo.png)

 ## Introduction
본 핸즈온 문서는 VMWare Tanzu Application Platform 에 대한 전반적인 내용과 실습을 위한 가이드 문서입니다. 본 과정에서는 Tanzu Application Platform의 제품에 대한 소개와 실습을 포함하고 있습니다. 
본 과정의 스크린 캡쳐 및 커맨드는 윈도우즈를 기준으로 작성되었습니다.

## Objectives
본 핸즈온 과정에서는 다음과 같은 내용을 학습하고 이해하는 것을 목표로 합니다.
* TAP (Tanzu Application Platform) 개요
* TAP을 이용한 앱 배포 방법
* 개발 IDE 도구에서 앱을 동적으로 배포하고 디버깅 하는 방법
* API Gateway 연결
* TAP의 Supply Chain을 이용한 파이프라인에 테스트 및 이미지 스캐닝 추가

## Required Artifacts
* 인터넷 접속 가능한 PC
* 쿠버네티스 플랫폼 및 kubectl CLI
* TAP 설치
* VS Code 및 TAP Plugin
* SSH Terminal (windows Putty, macOS Terminal 등)

## Hands-On 순서
0. [실습 환경 체크](docs/check.md) 및 [환경 구성](docs/configure.md)
1. TAP 개요 및 앱 배포
   * [TAP를 이용해서 APP 배포하기](docs/deploy-with-cli.md)
   * [TAP GUI에서 배포된 워크로드 확인하기](docs/gui.md)
   * [Spring Boot & Application Live View 확인하기](docs/alv.md)
2. 개발 환경 개선을 위한 IDE 경험
   * [IDE에서 앱 동적 배포하기](docs/deploy-in-ide.md)
   * [원격 디버깅](docs/remote-debugging.md)
3. MSA를 위한 아키텍처
4. [API Gateway 연동](docs/api-gw.md)
5. Supply Chain 개요 및 [파이프라인 추가](docs/scc.md)

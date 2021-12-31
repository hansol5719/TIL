# 리눅스\_하둡\_스파크\_몽고DB

> Contents
>
> 
>
> - 가상환경 구성
> - 주피터 노트북 연결_GPU연결
> - 리눅스 환경에서 깃허브에 연결
> - 리눅스 명령어 
> - 하둡 이론-설치
> - HDFS 명령어
> - HIVE 설치, 명령어
> - 스파크 이론-설치
> - 스파크 명령어
> - 몽고DB설치 명령어
> - 몽공DB- 리액트(REACT) 



1. 가상환경 구성

​	1) 가상화란?

​		https://m.blog.naver.com/ilikebigmac/222009981745



​	2) 오라클 버추얼 박스

​	 	https://www.virtualbox.org/wiki/Downloads



   - 윈도우 PC 안에 작은 PC(논리적으로 구분) 설치한다고 생각

     VirtualBox 6.1.30 platform packages

     Windows hosts (윈도우)

     OS X hosts (맥OS ) >> Next 설치 끝



​	3)  가상환경에 리눅스 설치하기

- centos리눅스 설치

​		http://mirror.anigil.com/CentOS/7.9.2009/isos/x86_64/

​		CentOS-7-x86_64-DVD-2009.iso 설치

- centos iso 바탕화면에 배치

- virtual box 열기
  - 이름 및 운영체제
  - 이름 : linux, 머신폴더 : default, 종류 linux, 버전 red hat (64bit)
- 메모리 크기 : 2048mb (변경)



​	! Red hat 32bit로 나올때 bios 변경하는 방법

​	https://m.blog.naver.com/n_jihyeon/221099021710



- 파일크기 : 주피터 깃허브만 쓴다면? 10GB, 하둡 스파크 몽고DB 할거면 30GB
- 하드디스크 파일 종류 : VDI (디스크 이미지)

- 물리적 하드 드라이브 지정 : 동적 할당

- 시작 버튼 누르기
  - 시동 디스크 선택
  - 추가 버튼 선택
  - 바탕화면에 위치한 CentOS-7-x86_64-DVD-2009.iso 선택
- install centos 방향키로 enter



​	!  마우스가 핸들링 안될 때 host key 변경해야 함

​	\-  아래 방향 화살표 클릭 >>  키보드 설정 >> 호스트키 조합 : ctrl+alt >> 확인

​    \-  전원 끄고 설정 재설정

​		\- 설정 클릭 >> 시스템 >> 마더보드 >> 포인팅 자치:SUB 태블릿 변경 >> 확인

​		\- 설치 용약 >> 설치대상 >> 자동파티션 클릭 >> 완료

​		\- 소프트웨어 선택(VERY IMPORTANT)

​			\- GNOME 데스크 탑 >> 선택한 환경 기능(전부 선택) >> 완료

 

- 사용자 설정
  - ROOT 암호 및 사용자 생성
  - 설정 완료 후 재 부팅

- Lincesing 동의 클릭
  - 네트워크 및 호스트 명 : 이더텟 켬 >> 완료
- root 로 접속
- 장치 >> 게스트 확장 cd삽입 클릭
- 바로 실행
- 바탕화면에 vbox cd 모양 나타나면 열기
- 설치 관련 화면 팝업 뜨면, 상단 옆 프로그램 실행 클릭 >> 설치
- 재부팅



[꿀팁] 윈도우와 복사 붙여넣기 자유롭게 하기

- 터미널 창 열어서 whoami 출력 잘 되는지 확인
- 리눅스 창 상단메뉴 중 장치 클릭 >> 클립보드 공유 >> 양방향 클릭
- 윈도우 메모장 열어서 확인해 보기
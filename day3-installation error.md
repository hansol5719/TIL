# 설치 과정 중 오류 잡기

- VirtualBox 64bit 설치 중 Red hat 32bit로 나올때 bios 변경하는 방법

​	참고-[https://m.blog.naver.com/n_jihyeon/221099021710]

----------------------------------------------------------------------------------------------------------

- VirtualBox 'No bootable medium found! System Halted.'
- 원인 : 바탕화면에 위치한 CentOS-7-x86_64-DVD-2009.iso 파일 대신 다른 파일을 선택한 채 가상 머신 시작

------------------------------

- VirtualBox \'가상 머신의 세션을 열 수 없습니다\' 

<img src="C:\Users\hansol\Desktop\캡처1 - 복사본.PNG" alt="캡처1 - 복사본" style="zoom:60%;" />



- 원인 : Fasoo DRM Client for NHN Mobile Wix 프로그램
  - 네이버 e-book을 설치할 때 같이 설치한 프로그램인 것 같다..
  - 제거 후 VirtualBox 재실행 해보니 되었다

참고-[https://besttech.tistory.com/27]

--------------------------------------------




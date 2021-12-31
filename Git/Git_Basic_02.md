#### Git을 이용한 버전관리 작성자 등록 (딱 1번만) 

```bash
git config --global user.name <내이름>
git config --global user.email <Github에 사용할 이메일>
git config --global --list # 설정 확인
```



#### 폴더를 Git으로 버전관리 하겠다

```bash
git init
```



#### Working Directory -> Staging Area -> Commits

```
git add .
git commit -m "커밋 메시지"
```



#### 현재 Git이 관리하는 파일의 상태

```
git status
```



#### 버전 로그 보여줌(커밋 로그 보여줌)

```
git log
git log -p
git log --oneline
```



#### 원격 저장소 연결

```bash
$ git remote add <이름> <주소>
```



#### 원격 저장소 연결 여부 확인

```bash
$ git remote -v
```



#### 원격 저장소에 반영

```bash
git push <저장소 이름> <브랜치 이름>
git push origin master
git push -u origin master # 이후에 git push만 해도 실행 가능
```



#### 원격 저장소 클론

```bash
git clone <원격 저장소 주소> 
```

- 원격 저장소의 커밋 내역을 모두 가져와서, 로컬 저장소를 생성



#### 원격 저장소 풀

```bash
git pull <저장소 이름> <브랜치 이름>
```

- 원격 저장소의 변경 사항을 가져와서, 로컬 저장소를 업데이트

# Git

> Contents
>
> - Git 초기 설정
> - Git 명령어



1. Git 초기 설정

   - 누가 커밋 기록을 남겼는지 확인할 수 있도록 이름과 이메일을 설정

   ```bash
   $ git config --global user.name "이름"
   $ git config --global user.email "메일 주소"
   ```

   - 작성자가 올바르게 설정되었는지 확인

   ```bash
   $ git config --global -l
   또는
   $ git config --global --list
   ```



2. Git 명령어

- git init : 현재 작업 중인 디렉토리를 Git으로 관리

  * ```bash
    $ git init
    Initialized empty Git repository in C:/Users/hansol/git-practice/.git/
    ```



- git status : Working Directory와 Staging Area에 있는 파일의 현재 상태를 알려주는 명령어
  - Untracked : Git이 관리하지 않는 파일 (한번도 Staging Area에 올라간 적 없는 파일)
  - Tracked : Git이 관리하는 파일
    - `Unmodified` : 최신 상태
    - `Modified` : 수정되었지만 아직 Staging Area에는 반영하지 않은 상태
    - `Staged` : Staging Area에 올라간 상태



- git add : Working Directory에 있는 파일을 Staging Area로 올리는 명령어

  * ```bash
    # 특정 파일
    $ git add a.txt
    
    # 특정 폴더
    $ git add folder/
    ```



- git commit : Staging Area에 올라온 파일의 변경 사항을 하나의 버전(커밋)으로 저장하는 명령어

  - ```bash
    $ git commit -m "first commit"
    [master (root-commit) c02659f] first commit
     1 file changed, 0 insertions(+), 0 deletions(-)
     create mode 100644 a.txt
    ```

  

- git log : 커밋의 내역(작성자, 시간, 메세지 등)을 조회할 수 있는 명령어

  - ```bash
    $ git log
    commit 1870222981b4731d14ef91d401c68c0bbb2f6e7d (HEAD -> master)
    Author: kyle <kyle123@hphk.kr>
    Date:   Thu Dec 9 15:26:46 2021 +0900
    
        first commit
    ```

    

  


# 25.07.16


1. 기초 문법
   
   - touch : 파일 생성
   - mkdir : 새 디렉토리 생성
   - ls : 리스트
   - cd : change directory
   - start : 열기
   - rm : remove
   - pwd : 현재 위치 확인


2. 경로
   
   - / : 루트 디렉토리
   - ~ : 홈 디렉토리


3. 마크다운
   
   - code block : ` 3개 ```print(하윙)```
   - 링크, 이미지 : [] 대괄호 활용 [google](링크), ![이미지](링크)
   - 글꼴 : * 두개 **굵게**, * 하나 *기울이기* ~두개 ~~취소선~~
   - 수평선 : - 3개 아래 처럼
   - 마크다운 가이드 : https://www.markdownguide.org/basic-syntax/



---



# 25.07.17



1. git 활용
   
   - git init : 시작
   - git add 파일이름 or . : staging area 올리기
   - git status : staging area 확인
   - git commit -m '????' : Repository 저장
   - git commit --amend : commit 메시지 수정 (vim들어가서)
   

2. Remote Repository
   
   - 원격 저장소 GitHub
   - 원격 저장소 추가 : git remote add *origin* (GitHub링크)
   - 저장소에 자료 넣기 : git push *origin* master
   - git clone *origin* master : 복사해서 가져오기
   - git pull *origin* master : 변경사항 가져오기
   - .gitignore : 올리기 싫은거 git init 전에 만들기
   - git remote -v : 저장소 목록 보기
   - git remote rm *origin* : *origin*(저장소 이름) 삭제


3. Git Revert
   
   - git revert commit_id : 없던일로하기, 기록 남음
   - git revert commit_id1 commit_id2 commit_id3 : 여러개 없애기
   - git revert commit_id1..commit_id3 : 범위 지정해서 없애기
   - git revert --no-edit commit_id : vim 안열고 바로
   - git revert --no-commit commit_id : 바로 commit ㄴ, staging area에만 올림


4. Git Reset
   
   - git reset [옵션] commit_id : 되돌리기
   - [옵션] --hard : 기록 없이 삭제
   - [옵션] --mixed : [옵션]칸 비워도 적용 working directory에 남김
   - [옵션] --soft : staging area에 남김
   - git reflog : hard로 리셋했던 목록까지 확인 가능
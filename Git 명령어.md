#### Git name/email 변경
- git config --global user.name "본인 git 아이디"
- git config --global user.email "본인 git 이메일"

#### 현재 master 브랜치를 main으로 이름 변경
git branch -m master main

***

#### Git Push
-  **처음 Push 할 때**
1. git init
2. git add .
3. git commit -m "커밋 메세지"
4. git remote add origin "git repositories 주소"
5. git push -u origin main

- **처음 Push 이후**
1. git add .
2. git commit -m "커밋 메세지"
3. git push

#### Git Pull
- **처음 Pull 할 때**
1. git init
2. git remote add origin "git repositories 주소"
3. git pull origin main --allow-unrelated-histories

- **처음 Pull 이후**
1. git pull origin main

***

#### 연결된 Git Repositories 확인
- git remote -v

#### Git Repositories 주소 바꾸는 방법
- **바로 주소 바꾸는 방법**
1. git remote set-url origin 바꿀 repositories 주소

- **주소 삭제하고 변경하는 방법**
1. git remote remove origin
2. git remote add origin "바꿀 repositories 주소"

***

#### Git Branch 확인/생성/변경/삭제/이동 방법
- 확인 : git branch
- 생성 : git branch 브랜치명
- 변경 : git branch -m 브랜치명 새로운브랜치명
- 삭제 : git branch -d 삭제할 브랜치명
- 이동 : git checkout 브랜치명

***

#### 팀 프로젝트 Pull/Push
- **Pull 받는 방법**
1. git clone "git repositories 주소"

- **본인 Branch 생성**
1. git branch 브랜치명
2. git checkout 브랜치명

- **처음 Push 할 때**
1. git add .
2. git commit -m "커밋 메세지"
3. git push -u origin 브랜치명

- **처음 Push 이후**
1. git add .
2. git commit -m "커밋 메세지"
3. git push

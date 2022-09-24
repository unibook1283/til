# Github
- Github is a hosting platform for git repositories.
- github 쓰는 가장 큰 이유는 **collaborate**

<br>

### git clone "url"
- "url"의 git repo를 내 local machine에 복사한다.
- 모든 git history도 다 가져온다.
- git init과 같이, git repo가 아닌 directory에서 해야한다. git status로 확인을 해야겠지.
- git log 쳐보면 진짜 history도 다 있네.

<br>

### github repo 만들기
- local에 이미 repo가 있을때
    1. github에 새 repo를 만든다.
    2. local repo를 연결한다.
    3. 변경사항을 push한다.

<br>

- local에 만들어논 repo가 없을때
    1. github에 새 repo를 만든다.
    2. local에 clone한다.
    3. 작업을 한다.
    4. 변경사항을 push한다.

<br>

### remote
- destination url이라고 보면됨.

### git remote
- 이 repo의 remote를 list로 보여줌.
- -v 붙이면 더 자세한 정보 -> remote 이름과 url

<br>

### git remote add "name" "url"
- url을 name이란 이름으로 remote 추가.

<br>

### other commands
- git remote rename "old" "new"
- git remote remove "name"

<br>

### push in detail
- branch라는것은, local branch와 remote branch가 따로 있다.
- 그냥 push하면 local branch와 같은 이름의 remote branch로 가는데, 다음 명령어를 사용하면 다른 이름의 remote branch로도 보낼 수 있다.
- git push "remote" "local-branch":"remote-branch"
- ex) git push origin master:test

<br>

### git push -u origin master
- -u를 하면, 이 다음 push부터는 뒤에 origin master 생략 가능.

<br>

### existing repository를 github에 처음 push 할 때 계속 났던 오류
- 아, 처음에 existing repository에 git init하면 branch가 없구나. 옆에 (master) 또는 (main)라고 나오는건 그냥 껍데기네. 그래서 push하면 이렇게 나오는거구나.
```
82105@DESKTOP-PG940IG MINGW64 ~/OneDrive/바탕 화면/ex (main)
$ git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/unibook1283/exercise.git'
```
- 해결법 : commit을 한 번 하면, branch가 생김.
- 첫 commit을 하기 전에는 branch를 못 만들게 해놨네. () 안에만 바뀌고.
- 이런 문제가 생기면 git branch로 branch list를 확인하자.
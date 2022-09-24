# Git의 기초: add와 commit

### Repository란?
- 파일과 폴더를 tracking하고 관리하는 **git workspace**다.
- repo라고도 한다.
- 모든 git repository는 자신만의 history를 가진다.

<br>

### git status
- git repository의 상태에 관한 정보를 준다.
- git repository에서만 쓸 수 있다.

<br>

### git init
- 새로운 git repository를 만든다.
- git 관련 무언가 하기 전에 꼭 해야 하는 것.

<br>

### 주의!
- git repository의 **하위 폴더도 모두 git으로 관리**된다.
- git repo 안에서 또 git init을 하면 문제가 생길 수 있으므로, git init 하기 전에는 항상 git status로 git repository인지 확인하는 습관을 들이자.

<br>

> working directory -> (git add) -> Staging Area -> (git commit) -> Repository

<br>

### git add
- commit을 위해, 변경사항들을 grouping.
- commit의 intermediate step이라고 보면 됨.

<br>

### git commit
- commit : 앞서 말한 check point라고 보면 됨. (snapshot of repository)
- add된 것들을 모두 commit함.

<br>

### git log
- commit 했던 기록들을 보여줌.
- 커밋을 구분하기 위한 hash code가 있는데, 너무 길고 복잡하다.
- git log --oneline : log를 간결하게 볼 수 있음. 엄청 긴 commit message도 첫 줄만 나옴. hash code도 짧게. good
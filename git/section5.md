# About commit

### Atomic commits
- 가능하다면 커밋을 원자적으로 유지한다.
- 각각의 커밋이 한 가지 변화만 다루도록 한다.
- 그렇게 하는 것이 나중에 undo, rollback 하기 더 쉽다.
- git add를 적절히 써서 한 가지 일(변화) 단위로 commit 하라는 뜻.

<br>

### commit message : 현재형 vs 과거형
- commit message는 현재형으로 쓰라고 git 문서에 나와있음.
- 명령문으로 써라.
- ~ fixed, ~ changed, ~ updated 대신 fix ~, change ~, update ~
- 정해진 건 없다는데 그냥 현재 명령문으로 쓰는게 좋을듯.

<br>

### 긴 commit message
- git commit 이렇게만 치면 vim 창에서 commit message를 칠 수 있음.

<br>

### Amending commits
- 바로 직전의 커밋을 수정할 수 있음. 파일을 추가하거나 commit message를 고치거나.
- git commit --amend

<br>

### .gitignore
- git repo가 특정 파일과 디렉토리는 무시하도록 할 수 있음.
- commit 하고 싶지 않은 파일들..
    - API keys
    - os files
    - log files
    - dependencies & packages
- wildcard * 를 쓸 수 있음.
- directory는 이름 끝에 /를 붙여야 됨.   
ex) node_modules/
- gitignore.io 라는 사이트에서 프로젝트별 gitignore를 만들어주네. 참고할 만 함.
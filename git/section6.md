# branch
### having separate context!

<br>

### master branch
- default branch
- 가장 뼈대가 되는 브랜치로 사용한다. 
- source of truth.
- official branch.
- git에서는 master, github에서는 main이라고 부른다.

<br>

### head
- repo에서 현재 위치를 의미함.

<br>

### git branch
- branch list 출력

### git branch "branch-name"
- head 위치에 branch-name의 branch 생성

<br>

### git switch "branch-name"
- branch-name 으로 전환.
- 와, 이거 하면 켜논 파일도 바로바로 바뀌네. 이래서 깃깃하는구나.

### git switch -c "branch-name"
- 생성과 switch를 한번에.

<br>

### git branch -d "branch-name"
- branch를 삭제
- -D = --delete --force
- merge를 한 번도 하지 않은 branch는 삭제할 수 없구나. 그럴 때 쓰는 것.

<br>

### git branch -m "branch-name"
- branch 이름 변경

<br>

### .git이 HEAD와 branch를 저장하는 방법
- .git의 HEAD라는 파일을 보면 현재 HEAD의 위치를 문자로 가지고 있다.
- .git/refs/heads에 가보면 branch마다 파일이 있는데, 각각 현재 위치한 commit의 hash code를 가지고 있다. (git log의 hash code와 비교해보면 그러함.) commit을 pointing하고 있다고 보면 됨.
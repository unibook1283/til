# Fetch and Pull
### git branch -r
- remote branch를 보여줌. 실제로 local repo를 update하는 것은 아님. 그건 fetch.

<br>

### git checkout "remote"/"branch"
- remote의 branch가 가장 최근에 communicate한 시점으로 감.

<br>

### remote branch에 연결하기
- git clone해오면, local의 main branch만 remote의 main branch에 연결됨. 다른 remote branch들은 local branch에 연결이 안되어있음. 그걸 연결하려면, 그 local branch로 가서 git switch "remote branch이름"하면 됨.
```
$ git switch movies
Switched to a new branch 'movies'
Branch 'movies' set up to track remote branch 'movies' from 'origin'.
```

<br>

### Fetching
- pull은 working directory에 github repo의 변경사항을 당겨오는거고, fetch는 working directory는 그대로 둔 체, local repository에 당겨오는것.
- 강의자료의 diagram을 보면 이해가 잘 됨.

### git fetch "remote"

### git checkout "remote"/"branch"
- 말 그대로 checkout하는 것.
- ex) git checkout origin/main
- : origin remote의 main branch 변경사항을 working directory에 가져옴.

### Pulling
- 실제로 local repository를 udpate하려면 git pull을 하면 됨.
- git pull = git fetch + git merge
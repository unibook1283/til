# Merging Branch

여러 branch로 나눴으니 나중엔 다시 합치고 싶겠지.

### Key point!
1. We merge branches, not specific commits
2. We always merge to the current HEAD branch

a -> b로 merge 시키고 싶다면(a를 b에 덮어씀), b로 가서 a를 merge한다.
```
git switch (b)   
git merge (a)
```

### fast forward merge
- conflict가 발생하지 않는 경우. (그림 참고.)

<br>

### conflict during merging
1. conflict가 난 file을 연다.
2. conflict가 없도록 수정한다.
3. conflict marker도 지운다.
4. add하고 commit하면 끝.
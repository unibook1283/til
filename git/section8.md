# Git Diff

### git diff
- 아무 option 없이 쓰면, working directory를 staging area와 비교하여 변경 사항을 보여준다.

### git diff 결과 읽는법
```
diff -git a/index.html b/index.html
index fd8458..6fe893d 10644
--- a/index.html
+++ b/index.html
@@ -25,7 +25,7 @@
```
- a 파일의 25번 줄부터 7 line을, b 파일의 25번 줄부터 7라인을 가져왔다는 뜻.

<br>

### git diff HEAD
workign directory와 HEAD를 비교.
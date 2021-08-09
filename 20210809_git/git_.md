# Git Basic

## Git 시작하기

```bash
$git init
# 단일 텍스트 파일 만들기
$touch a.txt
$touch b.doc
$touch c.txt
# 폴더 만들기
$mkdir test_dir1
# 디렉토리 내 파일 확인. -al 은 숨긴 파일까지 다 보여줌.
$ls -al
# TXT 파일만 업로드할 수 ㅣㅇ'ㅅㄴ'
$git add "*.txt"
# 현재 Git 명령 상태 확인 commit 전 상태를 확인할 수 있음.
$git status
$git commit -m "text file commit"
$git status
# commit한 log 결과를 볼 수 있음.
$git log
# 폴더와 파일이 동시에 add
$git add b.doc /test_dir1 
$git commit -m "document and directory"
$git status
$git log
```

### Typora 설정 (이미지)

- Copy image to custom folder로 설정
- 폴더 명을 정하기... ```./md-images``` (폴더 이름 하고 싶은대로  )
-  Check Option Boxes
  - [x] 로컬 이미지에 위 규칙을 적용 
  - [x] 온라인 이미지에 위 규칙을 적용
  - [x] 가능하다면 상대적 위치 사용
  - [x] Auto escape image URL when insert



## Github global config

원격저장소 추가

```bash
# 원격저장소를 볼 수 있다. (verbose)
$git remote -v
origin  https://github.com/DHRyu227/TIL.git (fetch)
origin  https://github.com/DHRyu227/TIL.git (push)
```

```bash
$git remote add <원격저장소 이름 > <주소>
$git remote add origin https://github.com/<username>/<저장소이름>.git
```

- 원격 저장소(```remote```)를 추가해줘. ```Origin``` 이라는 이름으로 ```주소```를
- 이 주소를 origin으로 이름을 붙이는 것이다.

- 원격저장소가 이미 설정된 경우 설정이 되지 않는다.  \<remote origin already exist\>
  <지우고 다시 해야한다.>

# 원격저장소 삭제

```bash
$ggit remote rm <원격저장소 이름>
```



# 원격저장소 Push

```bash
$git push origin master
```

- git, push, origin master branch를...

- -u 옵션: upstream 옵션
  - git push 라고 명령을 하더라도 설정된 원격저장소에 브랜치를 push
  - git push -u origin master
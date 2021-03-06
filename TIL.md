# TIL

## Today I Learned

### 1.1 기본 기호

(<h#> 태그입니다</h#) <- 카테고리의 설정 / 폰트 크기와 다름

* 순서가 있는 목록 만들 수 있음
* ㅇ
* ㅇ
*  탭은 안으로 / shife + tab  은 바깥쪽으로



### 1.2 코드블럭

코드블럭 ``` + Enter 

```bash
$ git add .
$ git commit -m "first commit"
$ git push origin master
```

`강조` < `백틱으로 감싸줌



### 1.3 Image

- `![]()` 을 작성하고 `()` 안에 이미지 주소를 입력합니다. `[]` 안에는 이미지 파일의 이름을 작성합니다.

  

### 1.4 Link

- `[]()` 을 작성하고 `()` 안에 링크 주소를 작성하고 `[]` 안에 어떤 링크 주소인지 작성합니다.



### 1.5 Table

- `|` (파이프) 사이에 컬럼을 작성하고 `enter` 를 입력합니다.
- 마지막 컬럼을 작성하고 뒤에 `|` 를 붙여줍니다. |스페이스|

|      |      |      |      |      |      |      |      |      |      |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
|      |      |      |      |      |      |      |      |      |      |



### 1.6 기타

- `>` 을 입력하고 `enter` 키를 누릅니다.

> git은 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 분산 버전 관리 시스템이다.

- 인용문 안에 인용문을 작성하면 중첩해서 사용할 수 있습니다.

> $ git add .
>
> > $ git commit -m "first commit"
> >
> > > $ git push origin master



**수평선**

- `---` , `***` , `___` 을 입력하여 작성합니다.

**강조**

- 이탤릭체는 해당 부분을 `*` 혹은 `_` (언더바) 로 감싸줍니다.
- 보드체는 해당 부분을 `**` 혹은 `__` (언더바 2개)로 감싸줍니다.
- 취소선은 `~~` 표시를 사용합니다.

이것은 *이탤릭체*입니다.

이것은 **보드체**입니다.

이것은 ~~취소선~~입니다.


## Git Hub

### git 기초

수정 - 저장 - add - commit

1. git.init - git의 시작

2. git status - 현황을 보는 경우

   **Untracked files**:
     (use "git add <file>..." to include in what will be committed)
           a.txt (add 전에)

3. U - A 로 바뀜 add 한경우에 / git add a.txt

   **Changes to be committed**:
     (use "git rm --cached <file>..." to unstage)
           new file:   a.txt

4. commit

   $ git commit -m 'first commit'
   [master (root-commit) 914f261] first commit
    1 file changed, 0 insertions(+), 0 deletions(-)
    create mode 100644 a.txt

   옆에 U / A 사라짐 / **nothing to commit, working tree clean**

5. **git log** - 내용물 그자체를 보는 것 / 모든 커밋은 고유하다
   commit 914f26133ea2e7d531dc72966f6527ab141ca271 (HEAD -> master)
   Author: daehwnakim <hora546@naver.com>
   Date:   Thu Jul 7 15:42:44 2022 +0900

   **$ git log --oneline**
   914f261 (HEAD -> master) first commit

## github

- $ git remote add origin https://github.com/daehwnakim/push-test.git

- $ git push origin master

## commit 수정하기

- git commit 쓰고 - i (insert mode) - 수정 - :wq

## clone / pull

- git init 과 git clone [https] 는 한번 만하는 것 / 
- clone 은 remote 된 상태까지 불러옴 
- pull은 리모트 설정이 되어있을 때 업데이트사항을 다운로드
-  git pull명령은 원격 저장소의 내용을 가져와서 현재 브랜치와 병합(merge)까지 해주기 때문에

## gitignore

- gitignore.io 에서 관련 부수파일들을 push하지 않게 하는 것

## Branch

- 가지로 하나 추가 / 평행우주같은 느낌

-  브랜치 목록 확인
  git branch

  #새 브랜치 생성
  git branch [branch name]

  #특정 브랜치 삭제
  git branch -d [branch name]
  git branch -D [branch name]  # 강제 삭제(병합되지 않은 브랜치도 삭제)

  git switch [branch name]  # 다른 브랜치로 이동
  git switch -c [branch name]  # 브랜치를 생성함과 동시에 이동

   한 줄로, 모든 브랜치의, 그래프를 포함하여 커밋 목록 출력
  git log --oneline --all --graph

   브랜치 병합
  git merge [branch name]

  git switch [branch name] = git checkout [branch name]















# 7 / 15 REVIEW
## Git : 분산 버전 관리 프로그램
  - 코드의 히스토리(버전)를 관리하는 도구
  - 개발되어온 과정 파악 가능
  - 이전 버전과의 변경사항 비교 및 분석
  - Git(분산 버전 관리 프로그램) 와 Github(Git 기반의 저장소 서비스)는 다른것

---
## GUI(Graphic Use Interface)
 : 그래픽을 통해 사용자와 컴퓨터가 상호 작용하는 방식

## CLI(Command Line Interface) 
 : 명령줄 인터페이스

GUI는 CLI에 비해 사용하기 쉽지만 단계가 많고 컴퓨터의 성능을 더 많이 소모
수 많은 서버 / 개발 시스템이 CLI를 통한 조작 환경을 제공

### CLI 기본적인 명령어
 - touch : 파일을 생성하는 명령어
 - Mkdir : 새 폴더를 생성하는 명령어
 - ls : 현재 작업 중인 디렉토리의 폴더/ 파일목록을 보여주는 명령어
 - cd : 현재 작업 중인 디렉토리를 변경하는 명령어
 - start, open : 폴더/ 파일을 여는 명령어(start : window, open : Mac)
 - rm : 파일을 삭제하는 명령어
 	(-r 옵션을 주면 폴더 삭제 가능 (rm -r foldername/))

---
## 절대경로 vs 상대경로
 ### 절대경로
	- 루트 디렉토리부터 목적 지점까지 거치는 모든 경로를 전부 작성한것
	- 윈도우 바탕화면의 절대경로 - C:/Users/ssafy/Desktop

#### 상대경로
	 현재 작업하고 있는 디렉토리를 기준으로 계산된 상대 경로 
	- 현재 작업하고 있는 디렉토리가 C:/Users일 때 윈도우 바탕 화면으로의 상대 경로는 ssafy/Desktop

	- ./ : 현재작업하고 있는 폴더,  ../ : 현재 작업하고 있는 폴더의 부모 폴더
------

## Markdown
 - 텍스트 기반의 가벼운 마크업(markup)언어 (마크업 : 태그를 이용하여 문서의 구조를 나타내는것)
 - 문서의 구조와 내용을 같이 쉽고 빠르게 적고자 탄생
 - README.md 파일을 통해 오픈 소스의 공식문서 작성


### [string](url)
 - string은 보여지는 부분, url은 연결할 곳

### ![string](img_url)
- 이미지(image)
- 이미지를 삽입 ( 이미지의 너비와 높이는 조절할 수 없다.)

### 텍스트 강조

- **bold**
- *기울임*
- ~~취소선~~
- 수평선 --- 3개 이상
#### 참고용 
https://www.markdownguide.org/cheat-sheet

---
## Git 기본기
### README.md
프로젝트에 대한 설명문서
Github 프로젝트에서 가장 먼저 보는 문서
일반적으로 소프트웨어와 함께 배포
작성 형식은 따로 없으나, 일반적으로 마크다운을 이용해 작성

### repository : 특정 디렉토리를 버전 관리하는 저장소
 - git init 명령어로 로컬 저장소를 생성
 - .git 디렉토리에 버전 관리에 필요한 모든 것이 들어있음


## GIt 이용 코드 참고
- git init
- code . (vscode 실행)
- (터미널에서) touch README.md
- git status (현재 git에서 관리되고 있는 파일의 상태를 알 수있음)
- git add README.md
- git status
- git commit -m ‘first commit’ <- 기록
- (git commit -m “commit_message” (커밋 메세지는 자세하게!))
- git config –global user.name ‘name’
- git config –global user.email ‘address@naver.com’
- git commit -m ‘create README.md’
- git log
- (깃 삭제 : rm -rf .git)

### 커밋은 working Directory  , Staging Area   , Repository  이 3가지 영역을 바탕으로 동작
- working Directory : 내가 작업하고 있는 실제 디렉토리
- Staging Area : 커밋으로 남기고 싶은, 특정 버전으로 관리하고 싶은 파일이 있는 곳
- Repository : 커밋들이 저장되는 곳

### README.md 수정하기
 : README.md 파일을 수정하고 명령어 실행
 -git log : git의 commit history 보기
 -git diff : 두 commit간 차이 보기

- git remote add origin https://github.com/hunsang-you/my_repo.git
-  git push -u origin main

## vscode와 깃허브 연결

- git remote add origin {remote_repo}
- git push -u origin master

- m -rf my_repo/ (my_repo라는 폴더의 파일 삭제)


- git clone (repository 주소)  (.git . 하면 그 폴더에 저장)

- git remote add origin https://github.com/hunsang-you/my_repo.git
- git push -u origin main


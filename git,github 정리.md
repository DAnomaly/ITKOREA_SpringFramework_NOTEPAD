# GIT / GITHUB 총정리

## 0. 사용자 등록
	0) git bash 실행
	1) 유저이름 등록    	: git config --global user.name '유저이름'
	2) 유저이메일 등록 	: git config --global user.email '유저이메일'

## 1. 로컬 저장소 만들기
	1) 이동             	: cd C:\Users\PSH_WORK\java_workplace
	2) 로컬 저장소로 지정 	: git init
		▶ 로컬저장소로 지정되면 (main)과 함께 경로안에 '.git'숨김 폴더가 생성됩니다

## 2. 스테이징하기
	1) 골라서 스테이징 	: git add 폴더명
	2) 전체 스테이징	: git add .

## 3. 커밋하기 (로컬 저장소에 저장하기)
	1) git commit
	▶ Vim에 커밋메시지 작성   
	```
	▶ Vim 명령어
	1) i		: 삽입
	2) <ESC>	: 삽입 종료
	3) :		: 명령입력 준비
	4) wq		: 저장하고 종료
	```   
	1) git commit -m '커밋메시지'
	▶ Vim을 사용하지 않고 '커밋메시지'를 작성하고 commit하는 방법
	2) git commit -am 'zzz'
	▶ git add . 작업을 동시에 하는 commit
	3) git status		: 저장되지 않은 파일을 찾기

## 4. github의 원격저장소(origin)에 저장하기
0) 첫 작업시 순서 (pull ▷ push)
1) git remote add origin https://github.com/DAnomaly/ITKOREA_SpringFramework_JAVA.git
	: origin 경로를 추가
2) git pull 		: origin에 있는 내용 내려 받기
	▶ git pull origin main --allow-unrelated-histories : 
		현재 로컬저장소의 과거를 무시하고 origin의 내용 가져오기(첫 작업 필수)
3) git push origin main 	: origin에 내용 올리기

-----------

### 기타
1) clear 			: 콘솔창 내용 모두 삭제
2) git log 			: 커밋 로그 불러오기
3) touch my.txt 		: my.txt파일 생성
4) echo 'xxx' >> my.txt 	: my.txt에 xxx내용 쓰기
5) cat my.txt 			: my.txt에 있는 내용 불러오기

### 이클립스에서 GIT을 사용하기
1) Git Repositories, Git Staging 창을 추가하기
	: Window → Show View → Others.. → Git Repositories , Git Staging
2) Git Repositories에 Git을 넣기
	: Add Git Repositories를 통해 본래 만든 .git폴더를 추가

### 사용 팁
GIT을 설치하고 나면 폴더에서 우클릭시 'GIT Bash Here'이 생긴다   
이것을 이용하면 cd를 사용하지 않고 GIT Bash를 그 폴더 경로에서 시작하게 해준다


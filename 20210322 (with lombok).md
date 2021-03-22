2021-03-22
===========
## JAVA PROJECT : 05_class
* ex08_static
	* static : 정적인, 모든 인스턴스의 공유하는 데이터
	* static field : 클래스 필드
	* public static final : 정적인 고정된 변수
	* private 으로 생성된 Constructor

## JAVA PROJECT : 07_inheritance
* ex17_Object.ex01
	* Object obj = new Dog();
* ex17_Object.ex02
	* .toString()
	* .toString() 오버라이드
* ex17_Object.ex03
	* lombok lib추가하기
	* lombok 활용하기
* ex17_Object.ex04
	* .equals() 오버라이드
* ex17_Object.quiz01
	* Object의 equals(), toString() 오버라이드

## JAVA PROJECT : 08_exception
* ex08_exception_class
	* BankAccountException을 만들어 Exception활용하기
	* try-catch를 이용한 MainClass
	* throws를 이용한 MainClass2

## JAVA PROJECT : 09_collection
* ex01_generic
	* 제너릭 타입에 대해
	* 객체를 생성하거나 메소드를 호출할 때 타입을 지정
	* 클래스명<제너릭 타입>
* ex02_generic
	* 제너릭 타입 2개 이상 사용하기
* ex03_generic
	* 제너릭 타입 배열 받기
	* 제너릭 타입 배열 보내기
* ex04_generic_method
	* 제너릭 타입의 메소드

## lombok 사용방법
1. lombok 설치
	1. 명령 프롬프트 실행
	2. lombok.jar 파일이 있는 디렉터리로 이동
	```다른 방법으로 폴더에서 shift + 우클릭을 통해 PowerShell창을 여는 방법 또한 있습니다```
	3. java -jar lombok.jar
	4. lombok을 설치할 eclipse 경로를 선택
	5. Install / Update 클릭
2. lombok 설치확인
	1. eclipse/eclipse.ini 파일 (메모장으로 열어서 확인)
	2. -javaagent:C:\Users\PSH_WORK\programs\eclipse\lombok.jar 내용확인
	```
	※ 이클립스 이동 등 사유로 경로가 바뀌게 되면 이클립스가 작동하지 않습니다.
	   (javaagent의 경로를 새로 수정하여야 합니다)
	※ 경로에 공백이나 한글이 있어서는 안됩니다
	```
3. lombok 사용하기
	```프로젝트에 lombok.jar 라이브러리를 추가합니다```
	1. 프로젝트 우클릭 - [Build Path]▶[Configure Build Path...]
	2. Libraries ▶ Add External JARs... ▶ lombok.jar 추가
4. lombok 활용하기
	1. 생성자, Getter, Setter 등을 자동으로 완성시켜주는 라이브러리
	2. 클래스에 에너테이션을 추가합니다. 
		1) @Getter : Getter를 추가해 줍니다
		2) @Setter : Setter를 추가해 줍니다
		3) @NoArgsConstructor : 매개변수 없는 생성자를 추가해 줍니다. (디폴트생성자)
		4) @AllArgsConstructor : 모든 필드에 매개변수를 전달하는 생성자를 추가합니다
		5) @Data : Getter, Setter, 생성자 등을 추가해 줍니다.
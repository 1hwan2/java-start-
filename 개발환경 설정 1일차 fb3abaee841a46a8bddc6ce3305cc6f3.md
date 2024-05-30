# 개발환경 설정 1일차

JDK 1.8 오라클

(롱텀서비스)LTS 사후지원을 얼마만큼 하는가

왜 최신버전을 사용하지 않는가?

자바가 가장 크게 많이 바뀐 시점들 8 11 17

현업에선 자바 8 버전이 가장 많이 쓰임.

(cmd)명령프롬포트 위치 찾기 cd.. 은 뒤로가기 cd 는 앞으로

c\users\program files 라면 c 까지 가려면 cd.. cd.. 두번

c\ 에서 다시 저기까지 가려면 cd cd 두번

소스코드는 파일의 형태로 저장.

시스템 환경 변수 편집 클릭

옵션값 javac -version 이런느낌 자바 몇버전인지 알 수 있는 방법.

public class Hello {
    public static void main(String[ ] args) {
        System.out.println("Hello World!");
    }

}

시스템 환경 변수 편집 클릭

환경변수 클릭

아래 쪽 시스템 변수 새로만들기

변수 이름

JAVA_HOME

jdk 까지만 설정 디렉토리 찾기

path 더블클릭 후 새로만들기

%JAVA_HOME%\bin

번역 결과물은 class 파일

클래스 파일 열기는 

java Hello 이런식

이것을 출력이라고 부른다.

만약 기존파일을 수정 할 시 번역을 한번 더 해줘야 새로 컴파일이 됨.

(프로그램)위에서 부터 아래로 문장 하나씩 실행. > 흐름

개발자의 일 중 하나는 순서를 만드는 것.

psvm 메인 메소드 public static void main 시작점.

public class My {
public static void main(String[ ] args) {
System.out.println("IlhwanJang");
System.out.println("010-7124-0964");

}

}

D:\1h2java>java My
IlhwanJang
010-7124-0964

D:\1h2java>

출력을 하기 위해선 번역이 필요(윈도우에선) 

psvm 파일을 만들땐 무조건 .java 를 입력하고 만들어야함.

개발자 환경 구축

JDK와 JRE는 무엇인가?

**JDK(Java Development Kit)**

**JRE(Java Runtime Environment)**

JDK는번역하면 자바 개발 키트이다. 간단하게 설명하면 자바를 개발하는데 필요한 기능들이 들어간 것이다.

여기에는 물론 자바를 실행하는데 필요한 jre도 포함되어 있어서 jdk를 다운로드 받으면 jre 또한 포함되어 있다.

자바 프로그램 개발을 위해서는 바로 이 jdk를 다운로드 받아 자바 기능을 사용하고 컴파일 해야하는 것이다.

즉, 정리해보면 자바 프로그램을 실행시키는데 필요한 것이 바로 jre이고 자바 프로그램을 개발하는데 필요한 것이 jdk이다.

jdk를 다운로드 받으면 jre도 포함되어 있어 개발한 자바 프로그램을 실행시키는 것까지 가능하다.

JRE란 번역하면 자바 실행환경으로 자바 프로그램을 실행하는데 필요한 것이다.

즉, 자바 프로그램을 실행시키는데는 문제가 없지만 자바 프로그램을 코딩할 때 jdk가 아니라 jre를 사용하면 문제점이 생길 수 있다.

예를 들어 컴파일이 정상적으로 되지 않을 수도 있다.
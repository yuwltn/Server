## JPA(Java Persistence API)란?
> 자바 ORM 기술에 대한 표준 명세로 `JAVA`에서 제공하는 API<br>

자바 어플리케이션에서 관계형 데이터베이스를 사용하는 방식을 정의한 인터페이스이다.
ORM을 사용하기 위해 만든 인터페이스이다.
ORM이기 때문에 자바 클래스와 DB테이블을 매핑한다. (sql을 매핑하지 않는다)

## ORM이 뭘까?
ORM은 Object Relational Mapping의 약자로 OOP에서 쓰이는 객체라는 개념을 구현한 `클래스`와 RDB(Relational Database)에서 쓰이는 데이터인 `테이블`을 **자동으로 매핑(연결)** 하는 것을 의미한다. <br>
그러나 `클래스`와 `테이블`은 서로가 기존부터 호환가능성을 두고 만들어진 것이 아니기 때문에 불일치가 발생하는데, 이를 ORM을 통해 객체 간의 관계를 바탕으로 SQL문을 자동으로 생성하여 불일치를 해결한다.<br>
따라서 ORM을 이용하면 따로 SQL문을 짤 필요없이 객체를 통해 간접적으로 데이터베이스를 조작할 수 있게 된다.

## JPA를 왜 사용해야 할까?
JPA를 사용하면 SQL 중심적인 개발에서 객체 중심적인 개발이 가능하다.<br>
간단한 메소드로 CRUD가 가능해 생산성이 증가한다.<br>
기존에는 필드 변경시 모든 SQL을 수정해야 했지만 JPA는 필드만 추가하면 SQL은 JPA가 처리해서 유지보수가 쉽다.<br>
Object와 RDB간 패러다임 불일치를 해결한다.<br>

## JPA 동작과정
JPA는 애플리케이션과 JDBC 사이에서 동작한다.
개발자가 JPA를 사용하면 JPA 내부에서 JDBC API를 사용하여 SQL을 호출하여 DB와 통신한다.
즉, 개발자가 직접 JDBC API를 쓰는 것이 아니다.

### JDBC(Java Database Connectivity)
JDBC는 DB에 접근할 수 있도록 `JAVA`에서 제공하는 API이다.


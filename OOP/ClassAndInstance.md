### 클래스와 인스턴스

클래스는 기본 뼈대이고
인스턴스는 구체적인 "상태(변수)" 와 "행위(기능)"의 집합이라고 생각하자.

![classAndInstance](/img/classAndInstance.png)

위 카드를 생각해본다면

카드 클래스에 대표적으로 들어가야 할 것들이 있을 것이다.



* 1. 고객의 이름 (변수)

* 2. 카드 유효기간 (변수)

* 3. 카드 번호 (변수)

* 4. 정보 인식 기능 (메서드)

* 5. 정보 보안 기능 (메서드)



##### 그런데 고객 A, 고객 B, 고객 C 마다 가지고 있어야 할 정보들이 각기 다를 것이다.

이렇게 찍어낸 카드는 각기 다른 "상태와 행위"를 갖는다.


```java
VisaCard 고객 A = new VisaCard ( ) ; // 고객 이름 : A , 유효기간 06월/20년

VisaCard 고객 B = new VisaCard ( ) ; // 고객 이름 : B , 유효기간 05월/13년

VisaCard 고객 C = new VisaCard ( ) ; // 고객 이름 : C , 유효기간 12월/17년
```


인스턴스의 존재이유를 "서로 다른 상태를 가지게 하기 위해서!" 라고 생각하자!
인스턴스의 존재이유를 "서로 다른 개성을 존중하자!" 라고 생각하자.

공부하면서 그렇게 생각하는 것이 제일 간단하다고 느꼈다.

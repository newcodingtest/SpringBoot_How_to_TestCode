

<p><a href="https://github.com/Around-Hub-Studio/AroundHub_SpringBoot.git"><strong>출처</strong></a>에서 공유 받은코드입니다.</p>

# TDD

테스트 주도 개발

테스트를 먼저 설계 및 구축 후 테스트를 통과할 수 있는 코드를 짜는것



애자일 개발 방식 중 하나

-코드 설계시 원하는 단계적 목표에 대해 설정하여 진행하고자 하는 것에 대한 결정 방향의 갭을 줄임

-최초 목표에 맟춘 테스트를 구축하여 그에 맞게 코드를 설계하기 때문에 보다 적은 의견 충돌을 기대할 수 있음



## 목적

코드의 안전성 증가, 기능 추가시 및 변경하는 과정에서의  SIDE EFFECT 저하

해당 코드의 목적을 명확하게 표현



### JUnit

자바의 대표적인 테스트 프레임워크

단위 테스트를 위한 도구를 제공

어노테이션 기반의 테스트를 지원

단정문(Assert) 으로 테스트 케이스의 기댁ㅄ에 대해 수행 결과를 확인할 수 있음



## JUnit Jupiter

TestEngine API의 구현체로 JUnit5를 구현하고 있음

작성한 테스트 코드를 발견하고 실행하는 역할을 수행

개발자가 테스트 코드를 작성할 때 사용됨



## JUnit Platform

Test를 실행하기 위한 뼈대

Test를 발견하고 Test계획을 생성하는 TestEngine 인터페이스를 가지고 있음

Test Engine을 통해 Test를 발견하고, 수행 및 결과를 보고

각종 IDE 연동을 보조하는 역할을 수행(콘솔 출력 등)

(PlatForm = TestEngine API + Console Launcher + JUnit 4 Based Runner 등)



## JUnit Vintage

TestEngine API 구현체로 JUnit 3,4를 구현하고 있음

기존 JUnit3,4버전으로 작성된 테스트 코드를 실행할 때 사용됨



![Mixing JUnit 4 and JUnit 5 tests](https://igorski.co/content/images/wordpress/2018/05/JUnit5Architecture-1.png)



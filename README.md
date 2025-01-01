# event-nauts
event management platform with micronauts

## 왜 micronaut인가?
JVM 생태계에서 프레임워크를 선택한다고 하면 Spring Boot, Micronaut, Quarkus 이 세 개가 많이 보이는 것 같다.
1. Spring Boot
- 얘는 지금까지 많이 해봤고 E-PPMS 프로젝트에서도 진행하고 있기 때문에 스킵.

2. Micronaut
- 스프링 부트보다 조금 더 빠른 부팅(런타임 < 컴파일 타임), 적은 메모리 사용량, AOT 등 최적화 기능이 눈에 띔.
- 물론 스프링 부트가 10초 걸리는데 얘는 5초 걸린다고 해서 50%나 성능이 좋다라고 단언할 수 없고 여러가지로 확인해봐야 할듯.

3. Quarkus
- 쿠버네티스같은 컨테이너 환경에서 동작하는 애플리케이션을 만들 때 적합.
- 근데 데이터 접근 레이어(Panache?)가 까다롭다고?
- 특히 RedHat 기반 JavaEE 경험이 있는 사용자들한테 친숙하다고 하는 게 왠지 Spring 진영이랑 다른 길을 걷는 것 같아서 찜찜.

요즘같은 대 클라우드 시대에.. 클라우드 네이티브 애플리케이션을 만들 수 있는, 스프링 부트보다 발전된 프레임워크라고 하는게 눈에 띄었고(스프링 부트도 GraalVM 등이 나오면서 이 쪽으로 많이 발전하고 있는 것 같긴 함) 일단 micronaut으로 도전해보기로 했다.

https://docs.oracle.com/ko/learn/build-cloud-native-java-applications-with-micronaut-and-graalvm/

학습 목적을 위해 코파일럿이 제안해준 이벤트 관리 프로젝트를 구현하면서 사용해보기로 함.

## Event Management Platform
Description: Build a platform for managing events, including event creation, registration, ticketing, and notifications.

Learning Points: This project will teach you about user notifications, scheduling, and handling high-traffic scenarios.


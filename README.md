# event-nauts
event management platform with micronauts

## 왜 micronaut인가?
JVM 생태계에서 프레임워크를 선택한다고 하면 Spring Boot, Micronaut, Quarkus 이 세 개가 많이 보이는 것 같다.
1. Spring Boot
- 얘는 지금까지 많이 해봤고 E-PPMS 프로젝트에서도 진행하고 있기 때문에 스킵.

2. Micronaut
- 스프링 부트보다 조금 더 빠른 부팅(런타임 < 컴파일 타임), 적은 메모리 사용량, AOT 등 최적화 기능이 눈에 띔.
- 물론 스프링 부트가 10초 걸리는데 얘는 5초 걸린다고 해서 50%나 성능이 좋다라고 단언할 수 없고 여러가지로 확인해봐야 할듯.
- https://micronaut.io/2020/04/07/micronaut-vs-quarkus-vs-spring-boot-performance-on-jdk-14/

3. Quarkus
- 쿠버네티스같은 컨테이너 환경에서 동작하는 애플리케이션을 만들 때 적합.
- 근데 데이터 접근 레이어(Panache?)가 까다롭다고?
- 특히 RedHat 기반 JavaEE 경험이 있는 사용자들한테 친숙하다고 하는 게 왠지 Spring 진영이랑 다른 길을 걷는 것 같아서 찜찜.

어쨌든 요즘같은 대 클라우드 시대에 클라우드 네이티브 애플리케이션을 만들 수 있는, 스프링 부트보다 발전된 프레임워크라고 하는게 눈에 띄었다. 물론 스프링도 GraalVM 등이 나오면서 이 쪽으로 많이 발전하고 있는 것 같긴 한데... 일단 좀 더 스프링 스타일에 가깝다는 micronaut으로 도전해보기로 했다.

https://docs.oracle.com/ko/learn/build-cloud-native-java-applications-with-micronaut-and-graalvm/

학습 목적을 위해 코파일럿이 제안해준 이벤트 관리 프로젝트를 구현하면서 사용해보기로 함.

### Docs
어쨌든 자바 표준 API를 준수하는 프레임워크들이라 단순한 컨트롤러~서비스~리포지토리의 CRUD를 만드는 건 어렵지 않겠지만 일단 문서정도는 읽어보는 게 좋을 것 같다.
- [코어](https://docs.micronaut.io/4.7.3/guide/)
- [DB 접근(SQL)](https://micronaut-projects.github.io/micronaut-sql/6.0.2/guide)
- [DB 접근(DATA JPA)](https://micronaut-projects.github.io/micronaut-data/4.10.5/guide)
- [보안 설정](https://micronaut-projects.github.io/micronaut-security/4.11.2/guide/)
- ...

## Event Management Platform
Description: Build a platform for managing events, including event creation, registration, ticketing, and notifications.

Learning Points: This project will teach you about user notifications, scheduling, and handling high-traffic scenarios.


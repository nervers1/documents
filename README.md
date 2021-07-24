## 리액티브 프로그래밍 소개
#### 리엑티브 프로그래밍이 세상에 소개된 지는 꽤 오래됐다. 무려 1970년대에 리액티브 프로그래밍에 관한 학술 자료가 나왔다. 그리고 리액티브 프로그래밍에 사용될 수 있는 비동기, 이벤트 주도 프로그래미이 기술이 나온 지도 이미 오래다. 그런데 왜 지금까지도 주류로 올라서지 못한 걸까?
#### 아마도 리액티브 프로그래밍을 써야만 할 정도의ㅣ 대규모 서비스가 많지 않았기 때문일 것이다. 하지만 세상은 새로운 시대로 접어들고 있다. 스타트업도 문자 그대로 수백만 명의 사용자에게 컨텐츠를 제공할 수 있어야 한다. 전 세계의 고객을 상대해야 하므로 24시간 동안 끊임없이 운영돼야 한다. 또한 클라우드 환경에서 애플리케이션을 운영하는 것이 보편화되고 있어서 '문제가 생기면 서버를 더 투입하면 된다' 같은 예전 방식은 이제 통하지 않게 됐다. 개발자들은 기존 자원을 더 효율적이고 일관성 있게 사용하는 방법을 찾고 있으며, 그 해법이 바로 **리액티브 스트림**이다.
### [http;//www.reactive-streams.org/](http;//www.reactive-streams.org/)에 간단히 정리되어 있는 리액티브 스트림은 __발행자__와 __구독자__사이의 간단한 계약을 정의하는 명세다. 트래픽을 가능한 한 빨리 발행하는 대신에 구독자가 '난  10개만 더 받을 수 있어.'라고 발행자에게 알리는 방식으로 트래픽을 제어할 수 있다. 그러면 발행자는 10개만 더 보낸다. 수요조절을 떠올리면 된다.
### 기업 간 시스템을 발행자와 구독자 관계로 연결하면 시스템 범위의 __배압__을 적용할 수 있다. 성능이 획기적으로 개선되는 것은 아니지만 트래픽을 잘 조절해서 관리할 수 있는 장점을 누릴 수 있다. 리액티브 스트림은 아주 단순해서, 사실 애플리케이션 개발자가 직접 다루는 것을 추천하지는 않는다. 대신에 프레임워크의 기초를 이루며 상호운영성을 높이는 데 사용된다.
    ###__프로젝트 리액터__는 VM웨어에서 만든 리액티브 스트림 구현체다. 리액터를 사용하면 다음 특성을 따르는 리액티브 프로그래밍을 활용할 수 있게 된다.
- 논블로킹, 비동기 프로그래밍 모델
- 함수형 프로그래밍 스타일
- 스레드를 신경 쓸 필요 없는 동시성

---

layout: default
title: 코루틴(Coroutine)
parent: Kotlin
has_children: true
nav_order: 1
---



## 코루틴(Coroutine)이란?

코루틴(Coroutine)은 실행과 지연, 재개를 허용하는 비선점형 멀티태스킹을 위한 [서브루틴](https://kennethss.github.io/docs/cs/sub-routine/)을 일반화하는 컴퓨터 프로그램의 구성요소라고 할 수 있습니다.



### 코루틴에서의 루틴

- 메인-서브 루틴의 개념이 없고 서로가 호출 가능
- 루틴을 진행하는 도중 특정 위치로 돌아갔다가 원래 위치로 돌아와 루틴 수행가능
- 서브루틴의 진입점, 반환점이 하나라는 종속적인 단점을 코루틴에서는 종속적이지 않기 때문에 데이터를 주고 받을 수 있음

### 멀티태스킹

```
하나의 Task가 Scheduler로 부터 CPU 사용권을 할당 받았을 때, Scheduler가 강제로 CPU 사용권을 뺐을 수 없으면 비선점형 멀티태스킹이고, 뺐을 수 있으면 선점형 멀티태스킹이다.
```



비동기 또는 비 차단 프로그래밍이 새로운 현실입니다. 서버 측, 데스크톱 또는 모바일 애플리케이션을 만들 때 사용자 관점에서 유동적 일뿐만 아니라 필요할 때 확장 가능한 경험을 제공하는 것이 중요합니다.

Kotlin은 언어 수준에서 코 루틴 지원을 제공하고 대부분의 기능을 라이브러리에 위임하여 유연한 방식으로이 문제를 해결합니다.

보너스로 코 루틴은 비동기 프로그래밍에 대한 문을 열뿐만 아니라 동시성 및 행위자와 같은 다양한 가능성을 제공합니다.

### 성능상의 이점

멀티 스레딩의 작업의 경우 스레드가 OS를 통해 작업들을 관리[Context Switching](https://kennethss.github.io/docs/cs/os/context-switching/)한다



### 코루틴의 장점

- 경량 및 성능 이점
- 메모리 누수 감소



- CoroutineScope
- CoroutineContext
- Dispatcher
- launch(async



- Channel
- Flow
- Action
# 5. 형식 맞추기

코드 형식을 맞추기 위한 간단한 규칙을 정하고 그 규칙을 착실히 따라야 한다. 팀으로 일한다면 팀이 합의해 규칙을 정하고 모두가 그 규칙을 따라야 한다.

## 형식을 맞추는 목적

코드 형식은 중요하다. 오늘 구현한 기능이 다음 버전에서 바뀔 확률은 아주 높지만, 오늘 구현한 코드의 가독성은 앞으로 바뀔 코드의 품질에 지대한 영향을 미친다.

## 적절한 행 길이를 유지하라

일반적으로 큰 파일보다 작은 파일이 이해하기 쉽다.

### 신문 기사처럼 작성하라

독자는 위에서 아래로 기사를 읽는다. 소스파일도 신문 기사와 비슷하게 작성한다. 이름은 간단하면서도 설명이 가능하게 짓는다.

### 개념은 빈 행으로 분리하라

거의 모든 코드는 왼쪽에서 오른쪽으로 그리고 위에서 아래로 읽힌다. 일련의 행 묶음은 완결된 생각 하나를 표현한다. 생각 사이에는 빈 행을 넣어 분리해야 마땅하다.

### 세로 밀집도

줄바꿈이 개념을 분리한다면 세로 밀집도는 연관성이다. 즉 서로 밀접한 코드 행은 세로로 가까이 놓여야 한다.

### 수직거리

시스템이 무엇을 하는지 이해하고 싶은데, 이 조각 저 조각이 어디에 있는지 찾고 기억하느라 시간과 노력을 소모한다. 서로 밀접한 개념은 세로로 가까이 둬야 한다.

같은 파일에 속할 정도로 밀접한 두 개념은 세로 거리로 연관성을 표현한다.

### 변수선언

변수는 사용하는 위치에 최대한 가까이 선언한다. 우리가 마든 함수는 매우 짧으므로 지역 변수는 각 함수 맨 처음에 선언한다. 또한 루프를 제어하는 변수는 흔히 루프 문 내부에 선언한다.

### 인스턴스 변수

반면 인스턴스 변수는 클래스 맨 처음에 선언한다. 변수 간에 세로로 거리를 두지 않는다.

### 종속 함수

한 함수가 다른 함수를 호출한다면 두 함수는 세로로 가까이 배치한다. 또한 가능하다면 호출하는 함수를 호출되는 함수보다 먼저 배치한다.

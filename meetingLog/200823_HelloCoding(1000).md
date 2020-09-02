# Hello Coding

## Chapter 9

Date: 200823 (오전 10시)

Roles: let todaysRole = { 진행자: 규하님, 타이머: 폴님, 서기: 시영님, 리액션: 하정님}

Contents:


#### 1. 숙제 검토
 
오늘은 숙제가 없어서 숙제 검토는 생략.

 
#### 2. 각자 배운 개념 정리


2-1 하정님 내용 정리

a. 최장 공통 부분 문자열과 최장 공통 부분열의 차이가 무엇인지?
왜 숫자가 0으로 되다가 갑자기 쌓이는 거지 의문이 들었음(추후 설명)

b. 탐욕 알고리즘과 동적 프로그래밍의 어원은 어떻게 되는지?
동적 프로그래밍은 리처드 벨만이 1940년대에 처음 소개(Coin)한 용어임
공군 군인들이 수학하는 걸 싫어해서 벨만이 Process라는 단어보다 Programming이라는 단어를 사용해서 그렇게 됨.
탐욕 알고리즘은… ㅠㅠ

2-2 폴님 내용 정리

a. 동적 프로그래밍의 내용은 지금까지 배운 내용 중 가장 흥미로운 내용이라 생각 함
동적 프로그래밍이 실질적으로 도움이 되는 프로그래밍이고
변수가 늘어나도 바로바로 업데이트 될 수 있다는 점이 실효성이 있어 보여 좋았음 

b. 폴님은 직접 따라해보고 테이블을 만드는 원리를 JS로 구현하는 방법을 따라해 보았다고 함


c. 폴님이 제시한 동적 프로그래밍 예시
아이템(책) 리스트를 추가할 때마다, 책마다 읽고 정도를 나타내는 가중치를 부여하고, 우선순위를 정할 수 있음 
새로운 아이템(책)이 리스트에 추가될 때마다 뭐를 먼저 볼 지 동적으로 업데이트 할 수 있었다는 점이 정말 좋았음 


2-3 시영님 내용 정리

a. 동적 프로그래밍에 대한 의견
“어려운 문제를 여러 개의 하위 문제로 쪼개고, 이 하위 문제들을 먼저 해결하는 방법”이라는 개념은 귀납법, Quick Sort와 같이 다른 알고리즘(학습 내용)에서도 많이 명시된 개념임
결국 알고리즘은 효율적으로 문제를 푸는 것을 추구하기 때문에 기본 개념은 비슷한 것 같음
격자로 나눠서 문제를 푸는 것이 신박하다고 생각

b. 파인만 알고리즘
- 문제를 작성한다
- 열심히 생각한다
- 답을 쓴다 
** 규하님 Comment : 파인만 아죠씨의 ‘참 쉽죠?’는 민철님이 제일 좋아하는 알고리즘임

2-4 규하님 내용 정리

a. 최장 공통 부분 문자열 vs 최장 공통 부분열

최장 공통 부분 문자열
- 똑같을 때만 카운트하고 값이 조건을 충족하지 않을 시 해당 부분은 0으로 기재
- 대신에 조건이 충족되는 경우가 발생할 시, 해당 값은 1로 기재하는 게 아니라 누적된 값을 기재 

최장 공통 부분열
- 각 부분별로 값이 누적 됨. 조건이 충족되지 않은 값일지라도 이전 값이 누적됨


b. 왜 지난 번에 탐욕 알고리즘 학습할 때 동적 프로그래밍이 중요하다고 언급했는지(폴님 질문)?

규하님 답변
- 양이 어마하게 늘어나서 동적 프로그램이 2^n으로 증가할 때 필요한 알고리즘이 탐욕 알고리즘임.
- 동적 프로그래밍으로 문제를 푸는 게 너무 비효율적이거나 불가능하다고 판단되면 탐욕 알고리즘으로 문제를 해결

c. 동적 프로그래밍을 빅오 개념으로 이해하려면(폴님 질문)?
- 동적 프로그래밍의 경우 빅 O 개념으로 단순하게 경우의 수를 정리하기에는, CasebyCase이기 때문에 정리가 어려움 


#### 3. 연습 문제 

- 폴님이 9-1번을, 서기 본인이 9-2번, 그리고 하정님이 9-3번 문제를 풀었는데, 각자 정리된 방식이 달라서 하정님이 정리한 내용을 공유하겠습니다. 
<img width="451" alt="동적프로그래밍1" src="https://user-images.githubusercontent.com/60086874/91675922-08d57b00-eb79-11ea-9d86-f05e353435f8.png">

#### 4. Assignment

- 추가로 작성할 코딩은 없음
- 오후 4시까지 KNN 알고리즘을 공부 해올 것 
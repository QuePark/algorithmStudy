# Hello Coding

## Chapter 10 KNN 알고리즘

Date: 200823 (오후 4시)

Roles: let todaysRole = { 진행자: 하정님, 타이머: 규하님, 서기: 시영님, 리액션: 폴님}

Contents:


1. 숙제 검토
 
오늘은 숙제가 없어서 숙제 검토는 생략.

 
2. 각자 배운 개념 정리


2-1 폴님 내용 정리

a. KNN 알고리즘 개념 및 유사도에 대한 기본 개념 설명

b. 거리 측정법에 대한 설명
피타고라스 정리를 사용
단순 x-y 축의 거리가 아닌, 다양한 특징들을 기준으로도 거리를 측정

c. Regression에 대한 설명 및 예시
규하님, 하정님, 폴님이 같은 취향을 갖고 있다고 가정
하정님이 다른 사람들보다 평점을 매길 때 가중치가 다르다고 한다면, 모두의 평균 값을 매겨서 평가 진행
빵집 예시가 좋았다고 생각 -> 꼭 X, Y축이 아닌 더 많은 특징들을 가지고도 정리할 수 있다는 점을 알 수 있어서 좋았음 

d. Cosine 유사도에 대한 설명 및 예시
사람마다 점수(평점)을 주는 기준이 다를 수 있기 때문에, 이웃간의 거리를 측정하기보다 두 벡터 사이의 각도를 측정하는 방식임

e. OCR에 대한 설명 
설명하기에 앞서 저자가 왜 갑자기 머신 러닝 개념을 소개했는지… 영리적인 의도가 있었지 않나 싶음(자기 책 팔려고)
OCR은 문자의 직선, 점, 곡선 등의 특징을 찾아내어 작성된 문자를 인식하고 분석함
구글에서 픽셀이라는 폰을 만들고 있는데, 그 내장 기술 중 어떠한 물체를 사진으로 찍으면 그게 인식이되어 무엇인지 확인해줌(이런 기술도 비슷한 원리라고 생각)
어떤 연예인이 입은 옷을 찾고 싶을 때 연예인의 사진을 분석하여 알아 맞추는 시스템이라고 이해

f. 가중치에 대한 개념 설명
KNN 알고리즘을 활용할 시 사람들의 수를 늘림으로서 가중치를 적용할 수도 있음
하정님이 최근 리액션 롤을 많이 맡으셨는데, 하정님의 롤을 결정할 때도 가중치를 부여할 수 있다...는 식으로 개념을 이해함

g. 스팸 필터
Naive Bayes Classifier
특징적 유사 정보를 규명해서 나눔
단어의 유사성을 찾아서 스팸 메일에 적용
네이버 노드를 찾는 개념이라고 생각하면 됨
스팸 메일에 바보라는 글자가 많다면 전부 검사를 함 
** 시영&하정님이 당근마켓과 크몽 등에서도 유사 기술이 적용 된 것을 본적있다고 코멘트

h. 폴님이 살짝 답답한 점
그래서 좋은 특징이란 무엇인지...와 관련된 내용이 부족했다고 생각

2-2 하정님 내용 정리

a. 구글 회원가입 할 때, Captcha를 보면 사진이 뜨고 신호등 사진들을 고르라고 할 때도 이 경우랑 같은건지 의문이 들었음
신호등의 특징만을 찾지 않았을지…(규하님이 맞다고 설명해줌)


2-3 규하님 내용 정리

a. 손글씨를 OCR이 분석한 내용을 공유
타일을 픽셀 단위로 쪼개서, 해당 픽셀을 Grouping함
어떤특정 포인트에 도달했을 때 어떠한 특성이 있다고 확인된다면 해당 내용을 기록 및 필터


<img width="397" alt="knn알고리즘1" src="https://user-images.githubusercontent.com/60086874/91691868-5a92fb00-eba3-11ea-95fa-39d253465377.png">
굴곡이 생겨 내려가는 포인트를 파란색으로


<img width="402" alt="knn알고리즘2" src="https://user-images.githubusercontent.com/60086874/91691876-5ebf1880-eba3-11ea-8dab-26d92af83413.png">
굴곡이 있어 내려가는 포인트는 노란색 등으로 나눠서 필터링을 함
필터링을 한 결과를 바탕으로 재분석하여 해당 문자를 재구성하고 어떤 문자인지 예측

b. 위 경우도 탐욕 알고리즘과 비슷한 개념이라고 보면 되는지(폴님 질문)?
좀더 근사 알고리즘과 유사한 개념이라고 생각하면 됨(규하님 답변)

c. 빵집 예시를 보면서, 규하님도 복순도에서 일 했을 당시 막걸리를 팔면서 날씨, 주말/휴일 여부, 방송 관련 내용이 있는지 여부 등을 나눠서 테스트를 했다고 함
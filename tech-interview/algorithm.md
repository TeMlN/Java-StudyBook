## 재귀 함수
재귀 함수란 자신을 다시 호출하여 작업을 수행하는 방식의 함수

피보나치 수열, 팩토리얼을 구할때 등등 사용된다.

## 이진 탐색
검색 범위를 줄여 나가며 원하는 데이터를 검색하는 알고리즘

## 순차 탐색
데이터의 배열을 처음부터 끝까지 차례대로 비교하여 원하는 데이터를 찾아내는 알고리즘

## 버블 정렬
서로 인접한 두 원소를 검사하는 정렬하는 알고리즘

## 선택 정렬
주어진 배열중 최소값을 찾고 그 최소값을 첫번째 원소로 두고
다시 같은 작업을 반복하여 마지막 원소가 남을때까지 반복한다.

## 탐욕 알고리즘
선택의 순간마다 당장 눈앞에 보이는 최적의 상황만을 쫓아 최종적인 해답에 돋달하는 알고리즘

## 몬테 카를로 알고리즘
무작위로 난수를 생성한다
생성된 난수를 기반으로 사용해서 구하고자 하는 확률을 계산한다.
난수 생성이 무한에 가까워질 수록 우리가 원하는 정보의 실제값과 근사해진다.

## 최단거리 알고리즘
1. 출발 노드를 설정하고 이를 기준으로 각 노드사이의 거리를 저장한다.

2. 방문하지 않은 노드 중에서 가장 거리가 짧은 노드를 선택 한다.
3. 해당 노드를 거쳐가는 경우와 거쳐가지 않는 경우를 비교하여 최단거리를 갱신한다.

2번 3번 과정을 반복한다.

## 깊이 우선 탐색(DFS), 너비 우선 탐색(BFS)
그래프를 탐색하는 방법의 종류이다.
* #### DFS
최대한 깊이 내려간 뒤, 더이상 깊이 갈 곳이 없을 경우 옆으로 이동

* #### BFS
최대한 넓게 이동한 다음 더 이상 갈 수 없을 때 아래로 이동

## 피보나치 수열
두 수의 합이 바로 뒤의 수가 되는 수의 배열.
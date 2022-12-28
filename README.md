# graph-cloloring
 Computational Statistics project


algorithm - 이용한 알고리즘은 총 3가지. 
1. Greedy
2. Antcol
3. Backtracking
- 원래 작동방식 알고리즘을 이용하지 않고, 처음으로 해가 나오며 해당 해를 사용하는 방법으로 사용. 대부분 동일한 방법으로 Backtracking 알고리즘을 GCP에 이용. 

Simulation 
-각 알고리즘별로 5번 반복 측정한 후, 색칠하 컬러 수가 최소값인 경우를 채택 
1. 간단한 경우 각 알고리즘의 성능 비교 
2. 노드수는 동일하고(n=100) 그래프 연결성 증가하는 경우(a 증가) 각 알고리즘의 성능 비교 
3. 그래프 크기가 증가(n,a)하는 경우 각 알고리즘의 성능 비교 


timetable scheduling
- graph coloring를 활용항 실생활 문제인 timetable problem를 해결

<개선할 점>
좀 더 정확한 알고리즘들의 비교작업을 위해서, 시뮬레이션 단계에 동일횟수별 최소값을 산출하는게 아니라, 가장 오랜 시간이 걸린 알고리즘을 기준으로, 해당 시간만큼 다른 알고리즘들을 반복했을때 산출되느 최솟값을 비교하는게 적절해 보인다. 
예를 들어 n=100, a=4124인 경우 ACO 알고리즘은 15.0701sec 시간이 걸렸다. Greedy느 평균 0.0158sec 시간이 소요되었기 때문에, ACO 알고리즘 1번 수행하는 동안 나온 값과, greedy알고리즘을 100번 수행하여 나온 최솟값을 비교하는 방향이 적절한 비교이다. 

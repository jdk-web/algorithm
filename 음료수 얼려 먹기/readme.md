
<h1>문제 : 음료수 얼려 먹기</h1>

N X M 크기의 얼음 틀이 있다. 구멍이 뚫려 있는 부분은 0, 칸막이가 존재하는 부분은 1로 표시.
구멍이 뚫려 있는 부분끼리 상, 하, 좌, 우로 붙어 있는 경우 서로 연결되어 있는 것으로 간주한다. 이때 얼음 틀의 모양이 주어졌을 때 생성되는 총 아이스크림의 개수를 구하는 프로그램을 작성

얼음틀<BR>
00110<BR>
00011<BR>
11111<BR>
00000<BR>
<BR>
아이스크림 개수 : 3

* DFS를 이용한 문제 접근
1. 특정한 지점의 상, 하, 좌, 우를 살펴본 뒤에 주변 지점 중에서 값이 0이면서 아직 방문하지 않은 지점이 있다면 해당 지점을 방문
2. 방문한 지점에서 다시 상, 하, 좌, 우를 살펴보면서 방문을 다시 진행하면, 연결된 모든 지점을 방문
3. 1~2번의 과정을 모든 노드에 반복하면서 방문하지 않은 지점의 수를 센다.

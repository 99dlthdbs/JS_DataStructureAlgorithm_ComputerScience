# **트리(Tree)와 우선순위 큐(Priority Queue)**

최단 경로와 같은 고급 알고리즘 문제에서 많이 사용되는 자료구조이다.
활용 빈도가 높다.

### **트리(Tree)**

- 트리는 가계도와 같이 <span style="background-color: #8E83A9;">계층적인 구조를 표현</span>할 때 사용할 수 있는 자료구조다.
- 나무(tree)의 형태를 뒤집은 것과 같이 생겼다.

<br />

### **트리 용어 정리**

- 루트 노드(root node) : 부모가 없는 최상위 노드
- 단말 노드(leaf node) : 자식이 없는 노드

  <br />

- 트리(tree)에서는 <span style="background-color: #8E83A9;">부모와 자식 관계가 성립한다.</span>
- 형제 관계 : 같은 level을 가지는 노드 사이의 관계

<br />

- ** 깊이(depth) ** : 루트 노드에서의 길이(length)
- 이때, 길이란 <span style="background-color: #8E83A9;">출발 노드에서 목적지 노드까지 거쳐야 하는 간선의 수</span>를 의미한다.
- 트리의 높이(height)는 루트 노드에서 가장 깊은 노드까지의 길이를 의미한다.

<img
src="https://velog.velcdn.com/images%2Fkimdukbae%2Fpost%2Ffefd2e62-bc4f-427a-a364-2ebc0b0c5c70%2Fimage.png"
width="100%"
/>

<br />

### **이진 트리(Binary Tree)**

- 이진 트리는 <span style="background-color: #8E83A9;">최대 2개의 자식</span>을 가질 수 있는 트리를 말한다.

<br />

### **우선순위 큐(Priority Queue)**

- 우선순위 큐는 우선순위에 따라서 데이터를 추출하는 자료구조다.
- 컴퓨터 운영체제, 온라인 게임 매칭 등에서 활용된다.
- 우선순위 큐는 일반적으로 **힙(heap)을 이용해 구현**한다.

| 자료구조                    | 추출되는 데이터             |
| --------------------------- | --------------------------- |
| 스택(Stack)                 | 가장 나중에 삽입된 데이터   |
| 큐(Queue)                   | 가장 먼저 삽입된 데이터     |
| 우선순위 큐(Priority queue) | 가장 우선순위가 높은 데이터 |

<br />

### **우선순위 큐를 구현하는 방법**

- 우선순위 큐는 다양한 방법으로 구현할 수 있다.
- 데이터의 개수가 *N*개일 때, 구현 방식에 따른 시간 복잡도는 다음과 같다.

| 우선순위 큐 구현 방식 | 삽입 시간 | 삭제 시간 |
| --------------------- | --------- | --------- |
| 리스트 자료형         | O(1)      | O(_N_)    |
| 힙(Heap)              | O(_logN_) | O(_logN_) |

- 일반적인 형태의 큐는 선형적인 구조를 가진다.
- 반면에 <span style="color: red;">우선순위 큐</span>는 **이진 트리(binary tree)** 구조를 사용하는 것이 일반적이다.

<img src="https://velog.velcdn.com/images%2Fapril_5%2Fpost%2F453a942b-6b07-46e9-a072-34d55a2f82d3%2Fimage.png"
width="100%"/>

<br />

### **포화 이진 트리(Full Binary Tree)**

- **포화 이진 트리**는 리프 노드를 제외한 모든 노드가 두 자식을 가지고 있는 트리다.

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FdfWC2R%2Fbtq9LqomTS7%2Frt4Io0pCfqBCckCs92CNz0%2Fimg.png"
width="100%"/>

<br />

### **완전 이진 트리(Complete Binary Tree)**

- **완전 이진 트리**는 모든 노드가 왼쪽 자식부터 차근차근 채워진 트리다.

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fb7BofG%2Fbtq9Eilu1J5%2F0HNO2KiWkBxTvERSJGHla0%2Fimg.png"
width="100%"/>

<br />

### **높이 균형 트리(Height Balanced Tree)**

- 왼쪽 자식 트리와 오른쪽 자식 트리의 <span style="background-color: #8E83A9;">높이가 1 이상 차이 나지 않는 트리</span>다.

<span style="background-color: #8E83A9;"></span>

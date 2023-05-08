# 기초 웹 스터디 6주차
박스모델
-------
블록 레벨 요소 - 한 줄을 차지하는 박스(부모 요소의 전체 칸 차지)<br>
인라인 레벨 요소 - 자신만을 감싸는 박스

박스모델 요소
- margin -> border -> padding -> content
- content : 내용(직관적)
- padding : 컨텐츠와 border 사이의 간격
- border : 테두리
- margin : border로부터 다른 컨텐츠 사이의 여백

박스모델의 스타일을 바꿀때 top -> left -> bottom -> right 순으로 적용된다. <br>
4개의 값을 입력하면 순서대로,<br>
3개의 값을 입력하면 top -> left,right -> bottom순서<br> 
2개의 값은 top,bottom -> left, right 순서<br>
1개의 값은 모든방향에 한번에 적용된다.

Flexbox Layout (Flexiblebox Layout)
---
아이템이 배열된 방향인 '주축'을 정할 수 있다.<br>
주축과 수직한 축을 cross axis (주축: main axis) <br>
ex : row가 주축이면 column이 cross axis, 주축이 column이라면 그 반대 <br>
아이템이 특정 축에서 어떻게 정렬 될 지도 지정이 가능함. <br>
이때 justify-content 는 주축에 해당되고, align-items는 cross axis에 해당된다.

## Flex 과제
### Justify-content
- flex-end : 오른쪽 정렬
- center : 중앙 정렬
- space-around : 모든 item 균등한 간격으로 정렬
- space-between : 첫번째, 마지막 item은 좌우 정렬후, 균등한 간격으로 정렬
### Align-items
- flex-end : 바닥으로 정렬
- center : 중앙으로 정렬
### Flex-direction
- row-reverse : 텍스트의 반대 방향으로 정렬
- column : 위에서 아래로 정렬
- column-reverse, row-reverse를 사용하면 start,end의 순서도 바뀜
- flex-direction이 column이면 justify-content가 세로가 됨 (align-items는 가로가 됨)
### Flex-wrap
- wrap : 여러줄에 걸쳐 정렬
### Flex-flow
- flex-flow = flex-direction + flex-wrap <br> 두 기능을 동시에 사용하는 것
- flex-flow : column wrap - 세로로 여러줄에 걸쳐서 정렬

# 기초 웹 스터디 8주차

자바스크립트는 동적 타입 언어이기에 변수의 타입 지정을 안해도 됨.<br>
int float등 숫자를 구분하지 않고 그냥 number하나의 숫자 타입밖에 없음.

- undefined - 선언 이후 값을 할당하지 않은 변수가 가지는 값
- null - 의도적으로 변수에 값이 없다는 것을 명시할 때 사용
- symbol - 이름의 충돌 위험이 없는 유일한 객체의 프로퍼티 키를 만들기 위해 사용됨

변수설정
- 
- var 변수이름 = 변수<br>
let 변수이름 = 변수<br>
 const 상수이름 = 상수
- var, let : 선언 , 변수에 값을 할당
- var - 재선언 가능<br>
let, const - 재선언 불가능
- var, let - 재할당 가능<br>
const - 재할당 불가능

scope
- 
- var - function scope<br>
let , const - block scope (block = 중괄호로 묶인것들)

암시적 형 변환 <br>
ex) 0 == '0'(True) , '0' -> 0 <br>
0 == [] (True), , Numnet([]) = 0 <br>
'0' == [] (False), [].toString = '' <br>
===, !== -> (타입까지 비교)

Protype
- 
- 자바스크립트에서 모든 객체는 자신의 부모 역할을 담당하는 객체와 연결되어 있음. 부모객체를 Protype 객체, 또는 Protype라고 함.
- 모든 객체는 [[Protype]] 이라는 인터널 슬롯을 가짐<br>
객체의 입장에서 자신의 부모 역할을 하는 프로토타입 객체를 가리킴
- protype 프로퍼티 - 함수 객체만 가지고 있는 프로퍼티, 이 함수를 통해 생성될 객체의 부모역할을 하는 객체를 가리킴
- constructor 프로퍼티 - 객체의 입장에서 자신을 생성한 객체를 가리킴

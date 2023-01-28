# CSS flex

flex 가 적용되는 요소는 `container`와 `item`로 구분할 수 있다.
`container`가 `item`들을 포함하는 형태이다.

display: flex 는 컨테이너에
flex: 1 1 100px은 아이템에 적용되는 속성이다

> `flex` CSS 속성은 하나의 플렉스 아이템이 자신의 컨테이너가 차지하는 공간에 맞추기 위해 크기를 키우거나 줄이는 방법을 설정하는 속성입니다.  
> `flex`는 `flex-grow`, `flex-shrink`, `flex-basis`의 단축 속성입니다. [_MDN Docs_](https://developer.mozilla.org/ko/docs/Web/CSS/flex)

flex-grow

- 0 이상의 값을 주면 확장한다.
- 아이템들의 값이 같다면 같은 영역을 차지한다

flex-shrink

- 아이템의 크기가 컨테이너를 넘어갈 때 줄이는 것과 관련한 속성
- 기본값 1 : 동등하게 줄어든다.
- 값 0 : 줄어들지 않는다.
  값 2 : 지정한 아이템이 2배 더 줄어든다.

flex-basis

- 컨테이너의 길이를 의미한다.
- 이는 flex direction에 따라 column이면 height, row면 width를 나타낸다.
- width, height 속성보다 flex-basis가 우선시된다.

flex

- 위 세 속성을 축약함
- flex : grow, shrink, basis

span은 영역을 갖지 못한다.
그와 다르게 영역을 갖는 요소들은 flex로 정렬하면 유용하다.

#### 컨테이너에 적용되는 속성은

방향

- property : flex-direction
- `row`, `column`, `row-reverse`, `column-reverse`

정렬

- property : justify-content 메인축의 정렬, align-items 교차축의 정렬
- value : `flex-start`, `flex-end`, `center`, `space-between`, `space-around`

# replaceSubrange(_:with:)

![스크린샷 2024-03-05 오후 8.07.32.png](replaceSubrange(_%20with%20)%20103a317d01998062aef4f7c9e0ac32af/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-03-05_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%2592%25E1%2585%25AE_8.07.32.png)

지정된 컬렉션의 요소로 요소의 범위를 바꾼다

말 그대로 **특정 범위에 대하여 elements를 대체**하는 자식..

**배열의 일부 요소를 다른 요소로 바꾸는 것**이라고 생각하면 된다!

---

[ Parameters ]

- subrange
    
    → 바꿀 배열의 범위, 범위의 시작과 끝은 배열의 유효한 인덱스여야한다
    
- newElements
    
    → 배열에 추가할(대체할) 새로운 요소
    

---

예시를 가져와봤다

![https://blog.kakaocdn.net/dn/cV2zx1/btsHsSZkGO7/2ZahRkFR98DYft6SmlM600/img.png](https://blog.kakaocdn.net/dn/cV2zx1/btsHsSZkGO7/2ZahRkFR98DYft6SmlM600/img.png)

먼저 subrange에 들어가는 범위는 인덱스가 들어간다

인덱스1 자리부터 인덱스3자리까지가 대체되어야 하고

뒤에 with 에 오는 "요소" 로 바꿔주는 건데 . . .

여기서는 1을 5번 반복하는 Element로 바꿔줘서

**[20, 30, 50] 에서 [1, 1, 1, 1, 1] 로 바뀌게된 것**
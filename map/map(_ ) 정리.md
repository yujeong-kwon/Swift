# map(_:)

![Untitled](map(_%20)%2058c64d650fd34339a89844946c751934/Untitled.png)

- 시퀀스 요소에 주어진 클로저를 매핑한 결과를 포함한 배열을 리턴한다
- [ Parameters ]
    
    transform → 매핑 클로저, 이 시퀀스의 요소를 매개변수로 받아들이고, 같거나 다른 타입의 변환된 값을 반환한다.
    

.

.

.

이게 무슨 말이냐면

배열안에 요소들을 매개변수로 받아들이고

정의한 **클로저의 형태에 맞게 일괄 처리한 배열을 반환**한다!

그렇기 때문에 for문보다 쉽고 간결하게 표현이 가능하다

나는 일괄 처리를 한다는 느낌으로 가장 잘 이해가돼서 적극 활용하고 있다

(map 이 뭔지도 모르고 인터넷에서 막 가져다가 썼던 과거를 반성하며,,,)

코딩을 한번 해보면 좀 더 이해가 되는데

```swift
//배열 [1,2,3,4] 에서 2씩 곱한 String으로 된 배열을 구하는 예제
let array = [1,2,3,4]
let multipliedArr = array.map({(value: Int) -> String in return String(value * 2)})
print(multipliedArr)

//추론하여 코드를 생략 가능, value의 타입 Int 와 return 키워드는 추론을 통해 생략 가능
let multipliedArr2 = array.map({(value) -> String in String(value * 2)})
print(multipliedArr2)

// 반환 타입도 생략 가능
let multipliedArr3 = array.map({(value) in String(value * 2)})
print(multipliedArr3)

//value는 여러번 사용하므로 $0으로 축약 가능
let multipliedArr4 = array.map({String($0 * 2)})
print(multipliedArr4)

//괄호도 생략 가능
let multipliedArr5 = array.map {String($0 * 2)}
print(multipliedArr5)

//만약 값에 문자열 "num: " 을 추가하고 싶다면
let multipliedArr6 = array.map {"num: \($0 * 2)"}
print(multipliedArr6)

//character형으로 변환된 result를 map을 사용하여 String형 배열로 변환
//>는 내림차순 정렬 <는 오름차순 정렬(디폴트임)
let arr: [Character] = ["1","2","3","a","f","0"]
let arrTest = arr.sorted(by: >).map({String($0)})
print(arrTest)
```

- $0은 첫번째 매개변수라는 의미
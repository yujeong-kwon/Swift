# reduce(::)

![https://blog.kakaocdn.net/dn/b1mUeX/btsHxDJCPcf/rFPEA3NofvL74XvpdVMgd0/img.png](https://blog.kakaocdn.net/dn/b1mUeX/btsHxDJCPcf/rFPEA3NofvL74XvpdVMgd0/img.png)

![https://blog.kakaocdn.net/dn/y9ai7/btsHxqKw6oV/ba8BgWe3bukUAXCafMmK71/img.png](https://blog.kakaocdn.net/dn/y9ai7/btsHxqKw6oV/ba8BgWe3bukUAXCafMmK71/img.png)

reduce는 고차함수의 종류 중 하나로, **주어진 클로저를 사용하여 시퀀스의 요소를 결합한 결과를 반환**한다

---

[ Parameters ]

- initialResult
    
    → 초기 누적 값으로 사용할 값으로, 클로저가 처음 실행될 때 initialResult는 nextPartialResult로 전달된다
    
- nextPartialResult
    
    → nextPartialResult 클로저의 다음 호출에 사용되거나 호출자에게 반환되기 위해 누적 값과 시퀀스의 요소를 새로운 누적 값으로 결합하는 클로저
    

---

**최종 누적 값을 반환**하며, 시퀀스에 요소가 없으면 결과는 InitialResult를 반환한다

joined()와 비슷하게 **누적하는 함수**로 활용하면 될 것 같다
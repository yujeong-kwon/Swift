# joined(separator:)

![스크린샷 2024-02-28 오후 1.11.57.png](joined(separator%20)%20103a317d019980508ac2fdd730546585/%25E1%2584%2589%25E1%2585%25B3%25E1%2584%258F%25E1%2585%25B3%25E1%2584%2585%25E1%2585%25B5%25E1%2586%25AB%25E1%2584%2589%25E1%2585%25A3%25E1%2586%25BA_2024-02-28_%25E1%2584%258B%25E1%2585%25A9%25E1%2584%2592%25E1%2585%25AE_1.11.57.png)

요소 사이에 **주어진 separator를 삽입하여 연결된 시퀀스를 반환**한다

---

[ Parameters ]

- separator
    
    → 시퀀스 요소 사이에 넣을 시퀀스
    

---

파라미터 separator를 넣어주면

문자열을 이어붙일 때 그 separator에 넣은 값을 끼워서 붙여준다

![https://blog.kakaocdn.net/dn/dvJqJe/btsHiprBgfk/XhSdrXKw8v1K6EBrkKyYQ1/img.png](https://blog.kakaocdn.net/dn/dvJqJe/btsHiprBgfk/XhSdrXKw8v1K6EBrkKyYQ1/img.png)

옵션을 안넣어주고 joined()를 하면 그냥 이어붙인다!!

위 코드에서는 components로 " "(공백)을 기준으로 문자열을 먼저 쪼개주고

그 쪼개진 것들을 주어진 separator로 이어 붙인거다
# readLine(strippingNewline:)

readline은 실제로 앱을 만들 때는 잘 사용하지 않지만

코테에서는 아주 흔하게 쓰이는 문법인데..

![Untitled](readLine(strippingNewline%20)%20b820ee1c89b748429cba656703a46188/Untitled.png)

**현재 줄의 끝이나 EOF 에 도달할 때까지 표준 입력에서 읽은 문자열을 반환**한다

반환값이 옵셔널타입인 것에 주의 하자!!!

(알고리즘 문제에서는 입력이 잘못 들어오는 일은 거의 없을 것이기 떄문에

보통 그냥 강제 언래핑을 해서 사용하는 것 같다!)

[ Parameters ]

strippingNewline 

→ true 일 경우, 개행 문자와 문자 조합이 결과에서 제거된다.

그렇지 않으면 개행 문자나 문자조합이 유지, 기본값은 true

---

strippingNewline 은 이름에서 알 수 있듯이 개행 문자를 떼어버릴지말지 결정해주는 파라미터인데,

디폴트 true이면 엔터 전까지의 문자열을 리턴하는 것이다
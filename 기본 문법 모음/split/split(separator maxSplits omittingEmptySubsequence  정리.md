# split(separator:maxSplits:omittingEmptySubsequences:)

![Untitled](split(separator%20maxSplits%20omittingEmptySubsequence%20103a317d0199804d8818f67a50eb3712/Untitled.png)

![Untitled](split(separator%20maxSplits%20omittingEmptySubsequence%20103a317d0199804d8818f67a50eb3712/Untitled%201.png)

주어진 요소와 동일한 요소 주변에서, 컬렉션의 가능한 가장 긴 서브시퀀스를 순서대로 반환한다

---

[ Parameters ]

- seperator
    
    → 분할되어야하는 요소, 해당 인자를 기준으로 문자열을 쪼갠다
    
- maxSplits
    
    → 문자열을 분리하는 최대 횟수, 앞의 seperator 인자를 기준으로 몇번을 쪼개는가를 뜻한다
    
- omittingEmptySubsequences
    
    → false인 경우 seperator의 인스턴스 마다 비어있는 하위 시퀀스 ("")를 반환하며,
    
    true인 경우는 비어있지 않은 하위 시퀀스를 반환한다. 기본 값은 true
    

---

seperator 파라미터에는 쪼갤 기준 문자열을 넣어주고

maxSplit으로 최대 쪼갤 횟수까지도 지정해 줄 수 있음

(maxSplits 인자는 넣어주지 않으면 있는 문자열을 다 쪼개지만

원하는 만큼 쪼개려면 옵션을 넣어주면 될 것 같다 !!)

-> 아래에 예시 코드도 있음

그리고 **components()와 split()을 비교**해보자면 

---

[ components() 와 split() 비교 ]

- return type
    
    components() 는 [String]을 반환
    
    split() 는 [Substring]을 반환    (-> String으로 사용하려면 map으로 일괄 변환해줘서 써도될듯)
    
- Foundation 프레임워크 import
    
    components() 는 Foundation을 import O
    
    split() 는 Foundation을 import X
    
- 성능의 차이
    
     split가 components 에 비해 성능이 좋다 (”” empty subsequence의 처리에 있어서 성능이 좋다)
    
    split은 omittingEmptySubsequence 파라미터의 bool 값에 따라서 변하지만
    
     components는 항상 empty subsequence를 돌려주게 되므로
    
    만약 space를 separator로 가졌을 때 쪼개려는 문자열에 빈 공간이 많다면
    
    그만큼 ”” empty subsequence를 반환하게 되므로 성능적으로 느리다고 한다
    

---

여기서 마지막 줄을 좀 더 쉽게 이해해보기 위해서 이것저것 찍어보았다

![https://blog.kakaocdn.net/dn/68XhP/btsHdfaU9xw/fKWKZBMaqW5eH9KmKvEDck/img.png](https://blog.kakaocdn.net/dn/68XhP/btsHdfaU9xw/fKWKZBMaqW5eH9KmKvEDck/img.png)

" "(공백)을 쪼개는 기준으로 가질 경우, 쪼갤 문자열에 빈 공간이 많다면

split()은 ""(empty subsequence)를 포함할지 안할지 정할 수 있지만(디폴트는 포함안함)

components는 무조건 포함하기 때문에 성능의 차이가 나는 것 같다!
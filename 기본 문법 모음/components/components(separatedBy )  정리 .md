# components(separatedBy:)

![Untitled](components(separatedBy%20)%20103a317d019980bca94fcc9289b3bbf4/Untitled.png)

주어진 separator로 나뉘어진 receiver의 하위문자열을 포함하는 배열을 반환

---

[ parameters ]

- separatedBy
    
    → string을 나눌 구분자
    

---

seperatedBy에 구분자 String을 넣어주면

그 String을 기준으로 문자열을 쪼개서 String배열을 반환한다

그런데 코테를 하다보니까 seperatedBy에 String 으로된 배열을 넣어주길래

배열로 쓰지않아도 잘 쪼개지는데 배열로 쓰는 이유가 뭘까,, 생각하다보니?!

배열에 넣었다는건 여러개를 넣을 수 있는 것이고

그렇다는건 구분자를 여러개로 줄 수 있는게 아닐까 싶어서 실험해봤다!!!!

![image.png](components(separatedBy%20)%20103a317d019980bca94fcc9289b3bbf4/image.png)

위와 같이 배열안에 여러개의 String을 넣어주면

**그 여러개를 기준으로 문자열을 쪼갠**다

**기준을 여러개로** 줄 수 있는 것..!

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
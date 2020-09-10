# Kotlin

findviewbyid()
--------------

kotlin에서 findviewbyid()를 하지않고 view의 id만으로 접근 가능  
 ➡ 같은 결과
> __차이점이 있나❔__
```
kotlin에서는 findviewbyid()를 사용하지 않아도 된다.
Kotlin Android Extension만 적용시키면, 레이아웃을 import 시키는 것만으로도 XML에서 정의내린 위젯들을 Id로 읽어들인다.
✔ findviewbyid()를 사용해도 문제는 없다
```

lifecycle
---------

AAC의 viewmodel은 수명 주기를 고려하여 UI 관련 데이터를 저장하고 관리
화면 회전과 같은 환경변화에서도 데이터를 유지

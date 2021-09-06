# Kotlin

findviewbyid()
--------------

kotlin에서 findviewbyid()를 하지않고 view의 id만으로 접근 가능  
 ➡ 같은 결과
> __차이점이 있나❔__
```
kotlin에서는 findviewbyid()를 사용하지 않아도 된다.
Kotlin Android Extension만 적용시키면, 레이아웃을 import 시키는 것만으로도 XML에서 정의내린 위젯들을 Id로 읽어들인다.
✔ findviewbyid()를 사용해도 문제는 없다]
```

최근에는 **databinding(뷰결합)** 이 권장됨</br>
✔ 더 빠른 컴파일</br>
✔ 쉬운 사용성</br>

lifecycle
---------

AAC의 viewmodel은 수명 주기를 고려하여 UI 관련 데이터를 저장하고 관리</br>
화면 회전과 같은 환경변화에서도 데이터를 유지</br>
구성 변경(예: 기기 회전)으로 인해 활동이나 프래그먼트가 다시 생성되면 사용할 수 있는 최신 정보를 즉시 수신
<img src = "https://user-images.githubusercontent.com/45004756/92677034-d0465600-f35d-11ea-9e0e-baccdd822298.png" width="250" height="300">

 ➡ 둘 다 onDestroy()가 호출됨 </br>
> __화면회전과 앱 종료 등을 어떻게 구분하지❔__

 `isFinishing() 메서드로 구분`
 1. 활동이 종료되는 경우 
      - onDestroy()는 활동이 수신하는 마지막 수명 주기 콜백이 됨
 2. 구성 변경으로 인해 onDestroy()가 호출되는 경우 
      - 시스템이 즉시 새 활동 인스턴스를 생성한 다음, 새로운 구성에서 그 새로운 인스턴스에 관해 onCreate()를 호출
 


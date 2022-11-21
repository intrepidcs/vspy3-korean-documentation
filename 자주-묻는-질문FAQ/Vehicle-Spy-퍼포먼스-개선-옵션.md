# Vehicle Spy 퍼포먼스 개선 옵션

저사양 PC에서 Vehicle Spy를 구동하시거나, Tx panel을 이용하여 메세지 송신시 설정한 주기보다 송신 되는 메세지 주기가 길어지는 경우 다음과 같은 방법으로 소프트웨어 퍼포먼스를 개선하실 수 있습니다.

Tools->Options에서 아래와 같이 Core loop 시간을 1ms로 조정해주세요.

![Tools->Options->Performance 탭](../.gitbook/assets/Options-Performance.png)

추가적으로 속도 향상을 원하시면 아래 옵션을 추가로 변경해주세요. (이 추가 옵션은 Vehicle spy 프로그램을 동시에두 개 이상 실행시에는 효과가 없습니다.)

1. _Tools->Options_의 _Performance_탭에서 _Core loop_ 글자를 더블 클릭합니다.
2. _Affinity_ 설정을 통해 Vehicle Spy 각 기능마다 어떤 CPU 코어를 쓸지 할당할 수 있습니다. \
   예를 들어 인텔사 듀얼코어는 0,2번이 실제 코어이고 1,3번은 hyperthread입니다. 이 경우 _GUI_와 _Core_에 같은 코어(0)를 그리고 _Hardware Rx_와 _Hardware TX_에 같은 코어(2)를 할당하시는 것을 추천드립니다. 인텔사 쿼드코어를 사용 중이시라면 각각에 0,2,4,6번 코어를 할당하시면 됩니다.

![Tools->Options->Performance 탭](../.gitbook/assets/Options-Performance2.png)

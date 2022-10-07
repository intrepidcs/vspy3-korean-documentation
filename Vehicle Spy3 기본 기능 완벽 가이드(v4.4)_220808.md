<h1>Vehicle Spy 3 Manual(KOR)</h1>
by Intrepid Control Systems Korea
<div style="page-break-after: always;"></div>

<h1>Version History</h1>
<h2> V4.2</h2>

- Appendix 1 DBC 파일 편집법 전체 수정
- Section 4-1 Export Database 아이콘 사진 추가
- 동영상 가이드 링크 수정  

<h2> V4.3</h2>

- 목차 형식 변경
- Section 6.3. neoVI FIRE2를 이용한 아날로그 값 측정법(eMISC 사용법) 추가
- Section 1.2. 데이터베이스 플랫폼 생성 및 데이터베이스(.dbc, .ldf, .arxml) 등록 파트에 arxml 등록법 추가 등 전체 수정
- Section 5 진단 통신 파트 추가
- Section 2.5. 장비 단독으로 저장한 데이터 추출 파트 최신 버전 기준으로 업데이트, 버전별 파트 세분화 등 전체 수정
- Section 2.1. Messages 메뉴에서 데이터 저장 파트 전체 수정
- 기타 잘못된 링크 수정

<h2> V4.4</h2>

- Version History 오타 수정
- 2.3. Capture Function Block을 이용한 메세지 저장법 파트 전면 수정(수정 중)
- 1.2. 데이터베이스 플랫폼 생성 및 데이터베이스(.dbc, .ldf, .arxml) 등록 파트에 db 확인법 및 편집 방법 링크 추가
- 6.3. VSB 파일 변환 방법 추가
- 2.1. Messages 메뉴에서 데이터 저장 파트 잘못된 설명 일부 수정-
- 잘못된 링크 수정

<div style="page-break-after: always;"></div>

<h1> 목차 </h1>

- [1. Vehicle Spy 3 Quick Start](#1-vehicle-spy-3-quick-start)
  - [1.1. 하드웨어 설정](#11-하드웨어-설정)
  - [1.2. 데이터베이스 플랫폼 생성 및 데이터베이스(.dbc, .ldf, .arxml) 등록](#12-데이터베이스-플랫폼-생성-및-데이터베이스dbc-ldf-arxml-등록)
  - [1.3. 메세지 모니터링](#13-메세지-모니터링)
- [2. 데이터 로깅](#2-데이터-로깅)
  - [2.1. Messages 메뉴에서 데이터 저장](#21-messages-메뉴에서-데이터-저장)
  - [2.2. Logging 메뉴에서 신호 저장법](#22-logging-메뉴에서-신호-저장법)
  - [2.3. Capture Function Block을 이용한 메세지 저장법](#23-capture-function-block을-이용한-메세지-저장법)
  - [2.4. 장비 단독으로 메세지 저장법](#24-장비-단독으로-메세지-저장법)
  - [2.5. 장비 단독으로 저장한 데이터 추출](#25-장비-단독으로-저장한-데이터-추출)
    - [2.5.1. VSB 파일 추출(3.9.3.15버전 이상)](#251-vsb-파일-추출39315버전-이상)
    - [2.5.2. VSB 파일 추출(3.9.2.19버전 이하)](#252-vsb-파일-추출39219버전-이하)
    - [2.5.3. 추출된 VSB 파일을 CSV, DAT, BLF 등의 파일 형식으로 내보내기](#253-추출된-vsb-파일을-csv-dat-blf-등의-파일-형식으로-내보내기)
- [3. 신호 분석](#3-신호-분석)
  - [3.1. 실시간 신호 값 보기](#31-실시간-신호-값-보기)
  - [3.2. 실시간 신호 그래프 보기](#32-실시간-신호-그래프-보기)
- [4. 송·수신 메세지 사용법](#4-송수신-메세지-사용법)
  - [4.1. 수신 메세지 생성 및 DBC 파일 생성](#41-수신-메세지-생성-및-dbc-파일-생성)
  - [4.2. 송신 메세지 보내는 방법](#42-송신-메세지-보내는-방법)
  - [4.3. 메세지 데이터 저장 파일 송신(Playback)](#43-메세지-데이터-저장-파일-송신playback)
- [5. 진단 통신(UDS/CCP/XCP)](#5-진단-통신udsccpxcp)
  - [5.1. 진단용 데이터베이스 설정](#51-진단용-데이터베이스-설정)
    - [5.1.1. ISO14229(UDS) 데이터베이스 등록](#511-iso14229uds-데이터베이스-등록)
    - [5.1.2. CCP/XCP 데이터베이스 등록](#512-ccpxcp-데이터베이스-등록)
  - [5.2. 진단 통신 변수 모니터링](#52-진단-통신-변수-모니터링)
  - [5.3. Diagnostics 메뉴를 이용한 UDS 진단](#53-diagnostics-메뉴를-이용한-uds-진단)
- [6. 자주 묻는 질문(FAQ)](#6-자주-묻는-질문faq)
  - [6.1. DBC 파일을 편집하는 방법](#61-dbc-파일을-편집하는-방법)
  - [6.2. Logging 데이터 통합/분할/맵핑 (VSB Editor)](#62-logging-데이터-통합분할맵핑-vsb-editor)
  - [6.3. VSB 파일 변환 방법](#63-vsb-파일-변환-방법)
    - [6.3.1. VSB에서 .csv, .asc, .blf 등의 포맷으로 변환](#631-vsb에서-csv-asc-blf-등의-포맷으로-변환)
    - [6.3.2. VSB에서 MDF(.dat, .mdf, .mf4) 포맷으로 변환](#632-vsb에서-mdfdat-mdf-mf4-포맷으로-변환)
  - [6.4. neoVI FIRE2를 이용한 아날로그 값 측정법(eMISC 사용법)](#64-neovi-fire2를-이용한-아날로그-값-측정법emisc-사용법)
  - [6.5. 케이블별 핀맵](#65-케이블별-핀맵)
  - [6.6. Vehicle Spy 퍼포먼스 개선 옵션](#66-vehicle-spy-퍼포먼스-개선-옵션)

<div style="page-break-after: always;"></div>

# 1. Vehicle Spy 3 Quick Start

이 가이드는 Vehicle Spy 3를 처음 접하는 고객을 위한 가이드입니다. 이 가이드를 통하여 CAN 메세지와 신호를 보는 방법까지 한번에 배울 수 있는 자료입니다.

Vehicle Spy 3는 다양한 기능이 많지만 현재 이 가이드는 처음 사용하는 고객을 위해서 만들어 졌기 때문에 간단한 기능만 소개합니다.

프로그램 최초 실행 시에는 라이센스 파일 등록이 필요합니다. 아래 화면의 'Add License File' 버튼을 눌러 구입 시에 제공받은 .lic파일을 등록합니다. 라이센스 등록 후 라이센스 만료일도 함께 확인 하실 수 있으며 이 때부터 프로그램을 정상적으로 사용 가능합니다. 

![License](img/2020-01-02-13-08-49.png)

라이센스 관련 문의 사항이 있으시다면 [여기서](#contacts) 하시면 됩니다.

<div style="page-break-after: always;"></div>

## 1.1. 하드웨어 설정

[링크](https://www.intrepidcs.co.kr/support_resources.html)의 장비별 사용자 간단 메뉴얼을 참조하여 장비를 올바르게 연결한 후 진행합니다. 

장비마다 상이하지만 보통 25pin 또는 26pin 커넥터 쪽으로 12V 전원을 인가해주시고 USB 케이블(Rad-Galaxy는 이더넷 케이블)을 사용하여 PC와 연결하시면 됩니다. 케이블별 핀맵은 [여기](http://www.intrepidcs.co.kr/uploads/2/5/0/1/25016645/icsk_%EC%BC%80%EC%9D%B4%EB%B8%94%EB%B3%84_%ED%95%80%EB%A7%B5.pdf)에서 확인 가능합니다. 

![장비별 사용자 간단 메뉴얼](img/2020-01-02-13-15-32.png)

CAN이나 LIN 통신 사용 시에는 아래 절차에 따라 장비의 Baud Rate을 알맞게 설정해주세요. Baud Rate은 연결하려는 ECU(DUT) 장비와 동일하게 설정합니다.

Vehicle Spy 3 상단 메뉴바의 ![NeoVi Explorer icon](img/2020-01-02-11-31-14.png)를 누르시거나 Setup->Hardware로 들어갑니다.

![NeoVi Explorer](img/2020-01-02-11-20-59.png)

1. 연결된 장비 이름을 선택합니다.
1. ‘Connect’ 버튼을 누릅니다. 
1. 설정 변경을 원하시는 네트워크를 선택합니다. (ex. HS CAN)  
1. 해당 통신의 사용하는 경우 "Enabled"를 체크하고 Baud Rate을 알맞게 설정합니다.
1. ‘Write Settings’ 버튼을 누르면 Hardware Setup에서 변경한 내용이 저장됩니다. (창 오른쪽 아래의 파란색 문구를 확인해주세요.)

이 설정은 하드웨어에 저장 되는 설정으로 처음 한 번만 설정하시면 됩니다. 또한 사용하시려는 Baud Rate이 장비 Default Baud Rate과 동일하다면 설정을 변경하지 않아도 됩니다.

※ [‘Hardware Setup’ 사용법 영상](http://screencast-o-matic.com/watch/coiwnsfw9P)

<div style="page-break-after: always;"></div>

## 1.2. 데이터베이스 플랫폼 생성 및 데이터베이스(.dbc, .ldf, .arxml) 등록

데이터베이스(.dbc/.ldf/.a2l 등) 파일을 등록하면 데이터를 의미있는 값으로 해독(Decoding)할 수 있습니다. 데이터베이스 파일이 없다면 이 단계는 넘어가셔도 됩니다.

데이터베이스 플랫폼은 데이터베이스 파일들의 묶음입니다. 이 플랫폼을 먼저 생성 후 해당 플랫폼에 데이터베이스 파일을 등록하면 됩니다.

1. 플랫폼을 생성하기 위해 상단 메뉴 바에서 ![](img/2022-01-04-15-48-02.png)를 클릭하거나 Setup->Setup Platforms로 이동합니다.
1. Add 버튼을 누른 뒤 플랫폼 이름을 입력하고 OK 버튼을 차례로 클릭합니다. 플랫폼 이름은 차종으로 입력하면 관리하기 편리합니다.<br>![](img/2022-01-04-16-09-17.png)
2. 상단 메뉴 바의 Platform을 2에서 설정한 플랫폼으로 설정합니다.  <br>![](img/2022-01-04-16-13-51.png)
3. 데이터베이스 파일을 등록하기 위해 ![](img/Network%20Databases%20icon.png)을 클릭하시거나 Setup->Network Databases로 이동합니다.
4. CAN 통신을 사용하는 경우, 좌측에서 사용할 CAN 채널 선택 후 Add..., DBC 버튼을 차례로 눌러 .dbc 파일을 등록합니다.
![](img/2022-01-04-16-21-27.png)
1. LIN 통신을 사용하는 경우, 좌측에서 사용할 LIN 채널 선택 후 Browse 버튼을 눌러 .ldf 파일을 등록합니다.  ![](img/2022-01-04-16-30-31.png)
2. ARXML 파일을 가지고 계신 경우, 상단의 ARXML/UEF/VSDB Support 탭에서 ARXML.. 버튼을 눌러 등록합니다. ![](img/2022-01-06-17-44-46.png)
3. 파일 등록이 끝났으면 빨간색 박스가 깜빡 거리는 ![](img/2022-01-04-16-24-53.png) 버튼 또는 ![](img/2022-01-04-16-25-23.png)를 눌러 플랫폼 설정을 저장합니다.

데이터베이스 등록 이후에는 Spy Networks->Messages Editor 메뉴의 Database 탭에서 등록한 데이터베이스에 정의된 내용을 확인할 수 있습니다. 이 메뉴는 읽기 전용으로 데이터베이스 편집을 원하시면 [6.1. DBC 파일을 편집하는 방법](#61-dbc-파일을-편집하는-방법)를 참고하시기 바랍니다.

<div style="page-break-after: always;"></div>

## 1.3. 메세지 모니터링

실제 CAN 메세지를 보는 방법과 해당 화면의 기본적인 기능을 설명 드리겠습니다.
왼쪽 윗부분의 Offline 옆에 있는 아래로 향하는 화살표를 누른 후 ‘Run with Transmit’을 클릭하면 실시간으로 값을 확인할 수 있는 상태(Online)가 됩니다. 

이 때 아래와 같은 경고 창이 뜰 수 있는데, Hardware Setup에서 장비의 Baud Rate을 알맞게 설정하셨다면([1.1. Hardware Setup](#11-하드웨어-설정) 참고) 아래 화면에서 "Use Hardware Baud Rates"를 눌러줍니다. 

![](img/Networks.png)

그리고 난 후 Spy Networks->Messages로 이동 합니다.
 
![Messages](img/2020-01-02-13-20-58.png)

현재 연결하신 CAN또는 LIN 에 해당하는 메세지가 위와 같이 나오는 것을 확인 하실 수 있습니다.
먼저 현재HS CAN라인을 통하여 4개의 메세지가 나오는 것을 확인하실 수 있고 이전 과정에서 DBC(LDF)파일을 등록하셨다면 위에서 보시는 바와 같이 ‘+’를 누르면 ‘-’로 바뀌면서 신호의 값도 확인이 가능합니다. 또한 메세지의 값에 보시면 파란색과 회색으로 표시가 되는 부분이 있습니다.
이것은 메세지의 데이터 값이 바뀌는 속도에 따라서 빨리 바뀌면 회색, 느리게 바뀌면 파란색, 아무 변화가 없으면 하얀색으로 표시가 됩니다.

현재 위의 화면에서 위쪽에 보이는 버튼 중 자주 사용하는 대해서 설명해 드리겠습니다.


<div style="width:90px"> 메뉴 | 설명 
-------------------------------- | ----
![Messages-Scroll](img/Messages-Scroll.png)                                              | 메세지가 시간의 순서대로 들어오는 것을 보실 수 있습니다.
![Messages-TimeAbs](img/Mesaages-TimeAbs.png) | 시간을 online한 시점부터 메세지가 들어오는 시점의 시간으로 표시가 됩니다. 
![Messages-Pause](img/Messages-Pause.png) | ‘Scroll’ 버튼을 이용해 메세지를 보다가 일시 정지하여 필요한 메세지를 분석 하실 수 있습니다. (정지된 상태지만 메세지는 계속 받고 있습니다.) 
![Messages-Save](img/Messages-Save.png) | [그림 6]에 있는 파란색 긴 박스 안에 위쪽 끝부분이 검정색으로 표시된 회색 막대가 보이실 것입니다. 이것이 버퍼를 나타내는 것이고 버퍼에 쌓인 메세지를 저장 할 수 있는 버튼입니다. 저장 경로는 오른쪽 상단 ‘Data’버튼을 클릭하면 확인 가능합니다. (버퍼의 크기는 offline 상태에서 하단에 ‘Setup’버튼을 눌러 Number Of Messages in History에서 조정할 수 있습니다.) 
![Messages-Erase](img/Messages-Erase.png) | 버퍼에 쌓인 메세지를 삭제하는 버튼입니다. 

</div>


또한 필터 사용법을 설명 드리겠습니다.


![Messages-Filter](img/Messages-Filter.png)
 
위에서 보시면 오른쪽 빨간색 박스에 ‘Filter’라는 항목에다가 내가 찾고자 하는 정보를 입력하면 그 메세지만 보이게 됩니다. 위의 경우 ArbID에 123과 234의 메세지만 나오도록 설정하였습니다. 이렇게 필터를 사용하게 되면 왼쪽 ‘Filter’ 버튼이 눌러져 있는 상태가 됩니다. 다시 ‘Filter’ 버튼을 클릭하면 필터가 해제됩니다. 

‘Filter’ 버튼아래에 보시면 ‘Custom 1-6’의 항목이 있는데 이것은 고객 개개인이 원하는 방식으로 필터를 설정하실 수 있습니다. 설정 방법은 먼저 원하는 Custom필터의 세 번째 열에 있는 것을 선택하게 되면 아래와 같은 화면이 나옵니다.
 
![Messages-CustomFilter](img/Messages-Custom%20Filter%20.png)

위에 보시면 이름을 변경하실 수 있고 Database에 등록되어있는 신호 중에서 내가 보고자 하는 신호를 더블 클릭하면 오른쪽 부분에 해당하는 메세지가 보이게 됩니다. 이렇게 다 선택하셨으면 Custom 필터의 첫 번째 열을 체크하시면 해당하는 메세지만 보이게 되실 것입니다.

※ [‘DBC파일 등록’과 ‘메세지 보기’사용법에 대한 동영상](http://screencast-o-matic.com/watch/cojXhzfa1a)

<div style="page-break-after: always;"></div>

# 2. 데이터 로깅

연결한 자동차 통신 라인에서 나오는 메세지와 신호를 저장하는 방법을 소개합니다.
	
## 2.1. Messages 메뉴에서 데이터 저장

Vehicle Spy3에서 제공하는 가장 간편한 데이터 저장법으로 Messages 메뉴의 버퍼에 저장된 메세지를 저장할 수 있습니다. 

Messages 메뉴에서 수신되는 메세지는 메뉴 좌측에 막대로 표시되는 버퍼에 저장됩니다. 검은 색 선이 현재 위치이며 흰색 부분이 비어있는 부분, 회색 부분이 차있는 부분입니다. 링버퍼 구조로 버퍼 공간이 모두 꽉 차면 가장 오래된 데이터부터 덮어쓰기됩니다.

1. 데이터 저장 전에 먼저 Setup...버튼을 눌러 버퍼 공간의 사이즈를 변경할 수 있습니다. Number Of Messages in History에 버퍼 공간에 저장할 메세지의 갯수를 입력하고 Close 버튼을 누릅니다. 오프라인 상태에서만 가능합니다.
2. Save 버튼을 눌러 버퍼 공간에 쌓인 메세지를 저장합니다. vsb, csv, blf, pcap 등의 형식을 지원합니다. 
3. Data 버튼을 누르면 데이터 저장 경로가 열립니다.

![](img/2022-02-03-16-30-45.png)

<div style="page-break-after: always;"></div>

## 2.2. Logging 메뉴에서 신호 저장법

PC에서 설정하신 신호만 저장하는 방법에 관한 내용으로써 먼저 ‘Measurement’ -> ‘Logging’으로 이동합니다.
 ‘Select Signals…’ 버튼을 클릭하면 아래와 같은 창이 나오게 됩니다. 
 
![Enter Signals](img/EnterSingals.png)

먼저 Signal Group Name에 선택되는 신호 그룹의 이름을 입력합니다. 그런 후 신호를 선택하기 위해서 화면의 좌측 편에서 신호가 있는 곳을 선택해 줍니다. 
예를 들어 .dbc 파일을 등록 하셨다면 ‘Database’를 선택하시면 되고 직접 메세지를 만들어서 신호를 정의 하셨다면 ‘Rx Messages’나 ‘Tx Messages’로 이동하시면 원하시는 신호를 찾을 수 있으실 것입니다.  찾을 때 편리한 기능은 ‘Find’라고 적힌 곳에 해당 이름을 입력하시거나 해당 ID를 입력하시면 손쉽게 원하시는 신호를 찾으실 수 있습니다. 신호를 찾은 후 더블 클릭을 하시거나 좌측 상단에 있는 ‘+’버튼을 누르시면 현재 창의 상단에 해당하는 신호가 추가가 되고 ‘-’버튼을 클릭하면 해당 신호를 삭제 하실 수 있습니다.  또한 ‘↑’와 ‘↓’버튼을 이용하여 신호의 순서도 정하실 수 있습니다.


다 선택하신 뒤(OK버튼을 눌러서 나오신 다음)  ‘Log This Signal Group’의 체크 박스를 선택해 주신 뒤 아래 항목들에 관해서 설정을 해주시면 됩니다. 
 
![Logging](img/Logging.png)

각 항목들에 대해서 설명 드리겠습니다.
 - Log at Constant Rate: 아래 Log Rat(초 단위)에 선택한 주기마다 모든 신호의 값을 저장
 - Log All Updates: 선택한 신호들 중 신호의 값이 장비를 통해 들어올 때마다 각각의 신호가 저장
 - Save when data changes only: 신호의 값이 변경될 때 마다 저장
 - Log file: 파일의 이름 설정하는 곳
 - Log File Creation Options: 파일이 저장될 때 이름에 시작한 시간을 표시하는 설정

아래의 ‘Start Logging’란과 ‘Stop Logging’란은 기본으로 ‘Online’과 동시에 데이터가 저장이 되고 ‘Offline’하면 데이터가 저장이 멈추도록 설정되어 있습니다.
만약 특정 이벤트가 발생한 뒤 시작을 원하신다면‘Start Logging’란에서 ‘Start On Equation’를 선택 후 ! [fx](img/x.png)버튼을 눌러 원하시는 이벤트를 설정하시면 됩니다.
(직접 ![Start Logging](img/StartLogging.png) 버튼을 눌러 시작하시기를 원하신다면 ![fx](img/fx.png) 버튼을 누른 후 ‘Expression’에 “0”을 입력하셔서 ‘Online’후 ‘Start Logging’버튼을 눌러 데이터를 저장 하실 수 있습니다.)

※ 모든 데이터를 저장하셨다면 저장경로는 Vehicle Spy 3우측 상단에 있는 ‘Data’버튼을 클릭하셔서 확인하실 수 있습니다.

<div style="page-break-after: always;"></div>

##  2.3. Capture Function Block을 이용한 메세지 저장법

어플리케이션에 따라 원하는 설정으로 메세지를 로깅할 수 있는 기능입니다.

1. Scripting and Automation->Function Blocks 메뉴 좌측 상단의 ![](img/2022-01-06-17-20-02.png) 버튼을 누르고 Capture를 선택하여 Capture Function Block을 생성합니다.

2. *Buffer*탭에서 *Filters…* 버튼을 눌러 내가 원하는 메세지만 선택하여 받을 수 있습니다. (모든 데이터를 저장할 때에는 설정할 필요는 없습니다.) Filters... 사용은 [1.3. 메세지 모니터링](#13-메세지-모니터링)의 커스텀 필터 설정 부분을 참조하시기 바랍니다.
3. *Start*탭에서 로깅 시작 시점을 설정합니다.  
 ![Capture-Start](img/Capture-Start.png)  
 각 항목이 의미하는 바는 다음과 같습니다.
 - Start Immediately: Online과 동시에 시작
 - Manual Start: 수동으로 시작 (아래 Function Block 시작 버튼을 누르거나 Graphical Panel 또는 다른 Function Block을 통해 시작할 때 사용.) 
  ![FunctionBlocks-Capture](img/FunctionBlocks-Capture.png)
 - Use Start Expression: 지정한 수식이 참이 되었을 때 시작
  ![Capture-StartExpression](img/Capture-StartExpression.png)

 - Start Immediately Embedded Only: 장비에 이 Capture Function Block을 이식한 후에 장비 전원이 들어 왔을 때 바로 동작하는 방식 (PC에서는 동작하지 않음)

4. *Stop and Trigger*탭에서 로깅 정지 시점 또는 트리거 시점을 설정합니다. 각 항목의 의미하는 바는 다음과 같습니다.

 - Collect in a circular buffer: ‘Messages’ 창에서 저장하는 것처럼 링 버퍼를 사용하여 ‘Buffer Size’의 크기 만큼 최근 메세지가 저장 됩니다. (즉, 50000으로 설정을 했을 때 최근에 들어온 메세지 50000개만 저장이 됩니다.)
 - Collect in a one-shot buffer: 메세지 저장이 시작된 이후 해당 설정 크기까지만 저장이 됩니다.
 - Collect before and after a trigger expression: 지정한 수식이 참이 되었을 시점의 앞 뒤를 로깅합니다.

4. *Storage*탭에서 로깅된 데이터의 저장 시점과 파일 포맷을 지정합니다. *Automatically save when complete* 또는 *Stream to disk*로 설정하여 사용하면 됩니다.
  ![Capture-Storage](img/Capture-Storage.png)

위 4가지 설정을 하셨으면 Online하셔서 원하시는 설정으로 데이터를 저장하시면 되고 저장된 경로는 우측 상단의 ![Data](img/2022-02-03-15-04-05.png)버튼을 클릭하시면 해당 경로가 나오게 됩니다.

※ 주로 많이 사용하는 저장 설정 (장기간 PC 에서 메세지 저장을 할 때)
1. ‘Start’ 항목에서 ‘Manual Start’로 설정 후 Start/Stop Hotkey를 원하시는 키로 설정합니다.
그리고 가장 중요한 ‘Automatically restart when complete’ 체크박스를 꼭 선택합니다.
2. ‘Stop and Trigger’ 항목에서 ‘Collect in a one-shot buffer’로 설정하고 Buffer Size를 한 파일당 저장할 메세지의 개수로 입력을 합니다.
3. ‘Storage’ 항목에서‘Automatically save when complete’로 설정하고 Storage File에서 해당 파일명을 입력합니다.
4. 위 설정을 다 했다면 Online을 하신 후 설정한 Hotkey버튼을 눌러 저장을 시작하고 다 하셨으면 다시 한번 눌러 저장을 정지하면 됩니다.


<div style="page-break-after: always;"></div>

## 2.4. 장비 단독으로 메세지 저장법

장비를 PC에 연결하지 않은 상태에서 장비 단독으로 데이터를 저장할 수 있는 방법에 대해 소개합니다. 이번 방식을 사용하면 다양한 방식의 데이터 저장방법을 동시에 병렬 구조로 데이터 저장이 가능합니다.

Measurement->Vehicle Scape DAQ로 이동합니다. 또는 아래의 File->Logon 화면에서 VehicleScape DAQ 버튼을 클릭합니다.

![Logon-VehicleScapeDAQ](img/Logon-VehicleScapeDAQ.png)]

아래 그림의 빨간 박스 부분에 알맞은 데이터베이스(dbc, odx, a2l등)가 불러와졌는지 다시 한 번 확인합니다. 필요한 경우 해당 버튼을 눌러 데이터 베이스를 추가합니다. 

dbc, ldf, arxml 파일 추가 방법은 [여기](#12-데이터베이스-플랫폼-생성-및-데이터베이스dbc-ldf-arxml-등록)를 참고하시기 바랍니다.

![VehicleScapeDAQ-DatabaseSetup](img/VehicleScapeDAQ-DatabaseSetup.png)
 

데이터베이스 설정을 확인 했다면, Standalone Logging탭으로 이동합니다. 여기서 로깅을 어떻게 할 지 설정할 수 있는데 각 항목에 대하여 설명 드리겠습니다.


![VehicleScapeDAQ-Standalonelogging](img/VehicleScapeDAQ-Standalonelogging.png)


1. 로그 파일의 이름을 설정하는 곳으로 옆의 체크박스(Append Time and Date to file name)를 선택하면 파일이 저장되는 시점의 시간과 함께 파일 이름이 생성됩니다.

2. 어떤 메세지를 저장할지를 선택합니다. ‘Log all bus messages’를 선택 시 장비로 들어오는 모든 메세지가 저장 되며 ‘Log only the items selected on the Channels tab’를 선택 시 Channels 탭에서 선택된 시그널만 저장됩니다.

Channels 탭을 잠시 살펴보겠습니다.

![](img/2022-01-07-14-43-25.png)

Clear 버튼을 누르면 하단 Results 창에 현재 등록된 플랫폼 내의 모든 변수가 출력됩니다. 또는 검색된 변수의 목록이 출력됩니다. 로깅을 원하는 변수를 더블 클릭 또는 드래그로 다중 선택하여 Selected 버튼을 누르면 변수들이 우측 Selected Channels for Test에 추가됩니다. 

UDS/CCP/XCP 변수를 로깅할 때에는 상단의 Polling setup에서 주기를 설정하고 변수들을 우클릭하여 Rate를 Low/Normal/High 중 하나로 선택합니다.

1. 로깅을 시작하는 방법에는 크게 3가지가 있습니다.

![VehicleScapeDAQ-Standalonelogging-Start](img/VehicleScapeDAQ-Standalonelogging-Start.png)

- Start immediately: 장비에 전원이 들어오는 즉시 데이터를 저장을 시작하는 방법
- Start when expression is true: 특정 이벤트가 발생 했을 시 데이터를 저장을 시작하는 방법

"Start when expression is true"를 선택하면 오른쪽 편에 수식공간이 생기고 그 아래에 3가지를 선택할 수 있는 체크박스가 나오게 됩니다. 
 
먼저 ![fx2](img/fx2.png) 버튼을 눌러서 수식이 참이 될 때 데이터를 저장하는 방법이 있고 아래 체크박스에 설정된 장비를 이용하여 데이터 저장의 시작점을 정할 수 있습니다.

<a name="fx"></a>수식을 설정하는 방법은 다음과 같습니다. 

![fx2](img/fx2.png) 버튼을 누르게 되면 아래 화면이 나옵니다. 

![StartExpression](img/StartExpression.png)

위의 화면처럼 어떤 신호가 100의 값을 가지면 종료를 하고자 할 때를 가정하여 설명 드리겠습니다.<br>
먼저 ‘Description’과 ‘Expression’란에 값이 들어가 있다면 ‘Clear’버튼을 눌러서 그 값들을 지웁니다. 그런 다음 선택할 신호가 있는 경로로 이동합니다. (현재 ‘Messages Editor’창의 ‘Rx Messages’에 추가한 신호를 선택, 만약 등록한 .dbc 나 .ldf 파일에 신호를 선택하길 원한다면Rx Messages’아래에 있는 ‘Database’를 선택) <br>
찾은 신호를 더블 클릭하면 위와 같이 ’Expression’란에 “{**신호이름**과 관련위치}”(Ex. {**Control_Signal (Value)** :in0-sig0-0})라는 신호가 입력됩니다. 그런 뒤 위의 화면처럼 해당 수식을 직접 입력해주면 됩니다. (위의 화면에서는 “=100”을 직접 입력 했습니다.) <br>
‘Description’은 말 그대로 이름을 정하는 것이기 때문에 크게 신경 쓰지 않으셔도 됩니다. 마지막으로 ‘OK’버튼을 클릭하시면 됩니다. <br>
‘Add Operator’에 보면 사용할 수 있는 다양한 수식이 나와있으니 참고 하시면 됩니다. 또한 수식 관련 설명은 위의 ‘Help’버튼을 이용하시면 확인하실 수 있습니다.


체크 박스 설명 

* OR neoVI MIC button press: neoVI MIC 장비의 버튼을 눌러 데이터 저장을 시작
* OR neoVI MOTE using HS CAN3(neoVI 3G): neoVI MOTE 장비의 버튼을 이용하여 데이터 저장 시작
* OR Push Button Pendant/ MISC 5 Trigger: MISC 5를 이용하여 데이터 저장 시작

‘OR neoVI MOTE using HS CAN3(neoVI 3G)’의 체크박스를 선택하면 아래에 neoVI MOTE 체크박스가 선택되고 아래에서 관련한 옵션을 설정하실 수 있습니다. (보통 기본 설정된 방식으로 사용하시면 됩니다.) 현재 위의 화면에는 HS CAN3라인에 NeoVI MOTE를 연결하여 동작하도록 설정되어 있습니다.


- Start using trigger expression: 특정 이벤트가 발생 시점으로 전과 후의 데이터를 저장하는 방법

![vssal-start2](img/vssal-start2.png)

 

4. 로깅을 중단하는 방법에 대한 옵션은 로깅 시작 방법(과정 3)에 따라 달라집니다. 
로깅 시작 방법(과정 3)으로 Start immediately나 Start when expression is true를 선택하게 되면, 아래와 같이 나옵니다. 

![vssal-stop](img/vssal-stop.png)

'Finish after collecting ~ messages'를 선택하면, 입력한 수 만큼 메세지 로깅 후 종료합니다. 'Restart the collection when finished'를 선택하면 우측의 수식이 참이 되었을 때 로깅을 종료합니다. 수식을 설정하는 방법은 [여기](#fx)를 참고해주세요.

로깅 시작 방법(3)을 Start using trigger expression로 선택하면, 아래와 같이 나옵니다.


![vssal-stop2](img/vssal-stop2.png)

‘Pre/Post Collection’을 선택하면 수식이 참이 되었을 경우 전후로 설정한 만큼 데이터를 저장하게 됩니다. 아래 항목에서 장비의 sd 카드 사이즈에 맞게 Card Size를 조절하고, 시간(By time)으로 전과 후를 저장할 것인지 메세지의 개수(By number of messages)로 전과 후를 저장할 것인지 선택 할 수 있고 그에 따라 우측에서 정확한 시간이나 개수를 정할 수 있습니다.
그리고 상단 가운데 있는 ‘One-shot Report’를 선택하면 수식이 참이 되었을 때 ‘Channels’탭에서 선택된 신호나 메세지를 한번만 저장하게 됩니다.

5. 4번 과정에서 로깅 중단 지점을 설정하였는데 데이터 저장이 끝났을 때 다시 로깅 시작 조건(2)을 기다릴 지 아니면 데이터 저장을 완전히 종료할지 선택할 수 있습니다.

![vssal-restart](img/vssal-restart.png)




이외에 사용되는 각종 다양한 기능들을 설명 드리겠습니다.

 - 동시에 여러 개의 데이터 저장방식을 설정하는 방법

 ![vssal-collection](img/vssal-collections.png)
 
좌측 상단의 ‘+’버튼을 이용하여 새로운 데이터 저장방식을 만들어 병렬로 여러 개의 각기 다른 데이터 저장을 동시에 하실 수 있습니다.

 - 차량의 시동이 꺼졌을 때 로거 장비에 사용되는 차량 배터리를 절약하는 방법(Sleep mode)

![vssal-power](img/vssal-power.png)
 
Power Management에서 'Never go to sleep'은 어떠한 상태에서도 데이터를 저장하는 설정이고, 
'Sleep when there's no bus activity'로 설정하면 입력한 초 만큼 장비로 메세지가 들어오지 않는 경우 장비가 대기 모드로 들어가고 메세지가 들어오게 되면 다시 메세지를 저장하게 됩니다.


모든 설정을 마치셨다면 마지막으로 Status reporting 부분의 LEDs 체크박스가 체크 되어 있는지 확인해주시고(로거 상태 확인을 용이하게 하는 옵션) 가장 아래에 있는 'Generate'버튼을 눌러줍니다. 

![vssal-statusreporting](img/vssal-statusreporting.png)

 
![coremini console](img/Coreminiconsole.png)

그러면 위와 같은 창이 뜨게 됩니다.

먼저 ‘Target Devices’에서 내가 사용할 장비의 이름과 S/N가 맞는지 확인해 줍니다. 그리고 ‘Storage’가 ‘SD Card’로 선택되어 있는지도 확인해 줍니다. 특별히 확인해 주셔야 할 옵션이 ‘Run After Download’체크 박스인데 이것이 선택되어 있으면 ‘Send’버튼을 눌러 아래 파란 박스처럼 ‘Success’라고 메세지가 나오는 즉시 바로 데이터 저장이 시작되고 ‘Run After Download’를 선택하지 않고 ‘Send’를 누르면 바로 실행이 되는 것이 아니라 장비의 전원을 분리했다가 다시 연결한 순간부터 데이터가 저장이 됩니다. 그리고 아래 파란 박스처럼 ‘Send’를 눌렀을 때 ‘Success’ 메세지를 확인하여 장비가 단독으로 사용하는 것이 제대로 설정이 되었는지 최종적으로 확인을 해 줍니다.

※ 장비의 빨간색 LED가 2-3번 깜빡일 동안 초록색 LED가 1번깜빡인다면 제대로 데이터 저장이 되고 있다는 것을 의미합니다.

led 점멸에 따른 상태는 [여기](https://cdn.intrepidcs.net/support/neoVIHardware/FIREneoLEDBlink.htm)서 자세히 확인 가능합니다.

<div style="page-break-after: always;"></div>

## 2.5. 장비 단독으로 저장한 데이터 추출

장비 SD Card내에 저장된 데이터를 추출해보겠습니다.

NeoVI FIRE나 RED 제품을 사용 중이신 경우 아래 사진처럼 장비의 SD 카드를 제거하여 SD 카드 리더기를 이용해 SD 카드를 PC와 연결합니다. 이외에 NeoVI FIRE2 등을 사용하시는 경우 장비에서 SD 카드를 제거할 필요없이 장비가 PC와 연결된 상태에서 그대로 진행하시면 됩니다. 
 
![sdcardremove](img/sdcardremove.png)

<div style="page-break-after: always;"></div>

### 2.5.1. VSB 파일 추출(3.9.3.15버전 이상) 

![](img/2022-02-03-15-56-46.png)

1. Tools->Extract/Export 메뉴로 이동합니다. 
2. Source가 올바른 장비 또는 SD 카드로 인식되어있는지 확인합니다. 인식되지 않은 경우 Refresh 버튼을 누르거나 소프트웨어를 재시작해보시기 바랍니다.
3. Output으로 추출된 데이터가 저장될 경로를 선택합니다.
4. Extract All Files를 누르면 SD 카드에 저장된 데이터가 VSB 파일로 추출됩니다.
5. 원하는 기간 또는 원하는 파일만 추출하기를 원하는 경우 기간과 파일을 선택한 후 Extract Selected Files(n)를 클릭합니다. (파일 선택은 neoVI FIRE2, Rad Galaxy 등 상위 장비에서만 지원됩니다.)

<div style="page-break-after: always;"></div>

### 2.5.2. VSB 파일 추출(3.9.2.19버전 이하) 

Tools->Extract/Export 메뉴로 이동합니다. 

아래와 같이 ‘Source Data’위치를 SD Card의 위치로 설정하고 ‘Output Data’를 불러올 위치로 선택합니다. ‘Extract to VSPY binary(.vsb)’ 버튼을 클릭하면 SD 카드 안에 저장된 모든 파일이 .vsb(Vehicle Spy3 형식의 파일)로 ‘Output Data’에 설정한 곳에 저장 됩니다.

- (아래 스크린샷 상 파란색 부분) 시간 바의 길이를 조절하여 원하는 날짜의 파일만 추출 가능합니다.
- (아래 스크린샷 상 초록색 부분) Refresh List 버튼을 누르면 SD 카드 내 파일을 확인할 수 있고 원하는 파일만 선택하여 Extract 버튼으로 추출할 수 있습니다. -> 이 기능은 NeoVI Fire2, Rad-Galaxy에서만 지원됩니다. 
 
![](img/Extract.png)

<div style="page-break-after: always;"></div>

### 2.5.3. 추출된 VSB 파일을 CSV, DAT, BLF 등의 파일 형식으로 내보내기

데이터를 추출시 기본 Vehicle Spy 형식인 VSB 포맷으로 추출됩니다. 이 형식을 csv, dat, blf 등의 원하는 형식으로 변환하여 내보낼 수 있습니다.

1. Extract/Export 메뉴 내 Export 탭으로 이동합니다.
2. 원하는 파일 형식을 ‘Signal Data’나 ‘Message Data’에서 선택합니다. ‘Signal Data’를 선택 시 오른쪽 화면에서 원하는 신호를 선택적으로 내보낼 수 있습니다.
3. Export 버튼을 누르면 Output Directory 경로에 지정된 형식으로 파일이 저장됩니다. View Output Directory 버튼을 눌러 저장 경로를 열 수 있습니다.

![](img/Export.png)


<div style="page-break-after: always;"></div>

# 3. 신호 분석

실시간으로 신호들의 값을 확인하거나 그래프로 보는 방법을 소개 합니다.

## 3.1. 실시간 신호 값 보기

실시간으로 선택한 신호들의 값을 확인하는 방법에 대해서 소개 합니다.
먼저 ‘Measurement’에서 ‘Signal List’로 이동합니다. 그리고 신호들을 선택하기 위해서 ‘Select Signals…’ 버튼을 누릅니다. 그리고 난 후 Page 9를 참조하여 원하시는 신호들을 선택합니다.  선택이 끝나면 ‘Online’ 을 하여서 선택한 신호들의 값을 확인하면 됩니다. 그리고   와  버튼을 이용하여 글자 크기를 조정할 수 있습니다.


![Singal List](img/SingalList.png)

위의 그림에서 ‘Signal List’창의 ‘Update’ 항목은 해당 신호를 포함한 메세지가 수신되거나 송신 될 때 ‘–‘  ‘|’  ‘/’  ’\’ 이렇게 변경이 되면서 신호들이 실시간으로 송·수신 되는 것을 확인할 수 있습니다. (선택한 신호를 가진 메세지가 송 수신되지 않는다면 해당 항목은 멈춰있게 됩니다.)


<div style="page-break-after: always;"></div>

## 3.2. 실시간 신호 그래프 보기

실시간으로 선택한 신호들의 그래프를 확인 하는 방법에 대해서 소개합니다.
 먼저 ‘Measurement’에서 ‘Signal Plot’으로 이동합니다. 그리고 신호들을 선택하기 위해서 ‘Select Signals…’버튼 누른 후 Page 9를 참고하여 원하는 신호를 선택합니다.

 
![Singal Plot](img/SignalPlot.png)

처음 신호를 선택하면 위와 같이 신호가 겹쳐서 나오게 됩니다. 각각의 그래프로 값을 확인하고 싶거나 그래프의 색깔 굵기 등 다양한 정보들을 변경하는 곳은  버튼을 누르면 됩니다.
이 버튼을 눌러 그래프의 선 굵기와 색깔 표시방법 등은 ‘Channels’에서 설정하실 수 있고 신호를 따로 보기를 하기 위해서는 ‘Plot’ 항목으로 가서 ‘Stack Legend’체크 박스를 선택하시면 됩니다. 또한 위와 같이 신호들의 값도 나타내고자 한다면 ‘Show Legend’체크 박스를 선택하면 됩니다.
그리고 X축 범위 설정은 ‘X Axis Span(S)’값에 원하시는 시간(초)을 입력하면 되고 Y축의 범위를 자동으로 설정하고 싶다면 Y축에서 마우스 오른쪽 버튼을 눌러 ‘Zoom to Fit’을 선택하면 자동으로 Y축이 조정됩니다.



※ [신호 분석 사용법 동영상](http://screencast-o-matic.com/watch/colii4htFp)

<div style="page-break-after: always;"></div>

# 4. 송·수신 메세지 사용법

다양한 신호들을 가진 메세지를 전송하거나 수신하기 위해서 해당 메세지를 정의하여 사용하거나 직접 DBC파일을 만들어 사용하는 방법을 소개 합니다. 먼저 ‘Spy Networks’에서 ‘Messages Editor’로 이동합니다. 관련 방법을 소개하기 전에 꼭 알아두셔야 할 4가지 항목을 소개하겠습니다.
 
- on Network: 어떤 채널에서 메세지를 만들 것인가를 선택합니다. 즉 내가 사용하는 통신을 정확하게 선택해 주셔야 합니다.
- Receive: 수신 메세지를 정의할 때 이곳에서 메세지와 신호를 만들 수 있습니다. 또한 DBC파일을 생성할 때에도 이곳에서 작업이 이루어 집니다.
- Transmit: 송신할 메세지와 신호를 만들 때 사용하는 곳입니다.
- Database: DBC파일을 등록한 상태에서 DBC의 정보를 확인 하는 곳입니다.

## 4.1. 수신 메세지 생성 및 DBC 파일 생성

수신 메세지와 그 신호를 정의하여 실제 메세지가 수신했을 때 정의한 것으로 표현되게 하는 방법과 그 정의한 메세지들을 DBC파일로 만드는 방법에 대해서 소개합니다. DBC파일을 가지고 있다면 그대로 사용할 수 있지만 DBC파일이 없고 그 정보만 가지고 있거나 DBC파일을 만들고자 할 때 해당 방법을 이용하면 손쉽게 사용할 수 있습니다.
먼저 ‘Messages Editor’에서 ‘Receive’로 이동합니다. 메세지를 생성하기 위해서 상단의 ‘+’버튼을 누릅니다. 그곳에서 해당 메세지의 이름과 ‘Arbitration ID(ArbID)’, 메세지 데이터의 크기 등을 입력하거나 아래의 항목에서도 입력할 수 있습니다. (아래 그림 참조)


![Messages Editor](img/MessagesEditor.png)


![Messages Editor2](img/MessagesEditor2.png)

 
신호를 생성하기 위해서는 먼저 아래 ‘+’버튼을 누르면 신호가 하나 형성이 되고 그 신호의 이름과 타입을 설정할 수 있습니다. 신호의 위치와 크기를 정하는 방법에는 2가지가 있습니다. 첫 번째 방법으로 신호의 위치는 위에서와 같이 파란색으로 표시된 중앙부분을 마우스를 누른 상태에서 이동하여 정할 수 있고 크기는 파란색끝부분을 눌러서 크기를 정할 수 있습니다. 두 번째 방법으로  버튼을 눌러서 시작점과 크기를 입력하는 곳에 직접 숫자를 입력하여 설정할 수 있습니다. 그리고 이곳에서 이 신호의 Format, 최대 최소값, 단위 값 등 다양한 정보들을 입력할 수 있습니다.
또한 ‘Scaling’으로 이동하여 Scaling Type을 ‘Linear mX + b’로 선택하면 원하시는 대로 스케일링 작업도 하실 수 있습니다.
(현재 왼쪽 그림은 실제 들어오는 값에 0.2를 곱하고 10을 더하여 신호의 값이 표현되도록 되어 있고 아래 항목에서는 소수점 한자리의 값으로 신호를 표시하고 단위는 %로 설정되어 있습니다.)


![Edit Signal](img/Edit%20Signal.png)
  

이렇게 원하는 설정대로 다 선택한 뒤 ‘Online’을 눌러 ‘Messages’ 창에서 확인해 보면 해당 메세지와 신호가 설정한 대로 보여지게 될 것입니다. 
마지막으로 DBC파일을 만들려면 일단 위와 같이 DBC파일에 들어갈 모든 메세지와 신호들의 정보를 설정한 다음 ‘Messages Editor’창의 상단에 있는 ![MessagesEditor-ExportDatabase](img/2021-10-14-10-33-10.png)버튼을 누르면 됩니다.



<div style="page-break-after: always;"></div>

## 4.2. 송신 메세지 보내는 방법

메세지를 송신하는 방법을 소개합니다.

먼저 ‘Messages Editor’에서 ‘Transmit’으로 이동합니다. 그리고 나서 이전 과정에서 설명한 '1. 수신 메세지 생성 및 DBC 파일 생성’을 참고하여 동일한 방법으로 송신할 메세지와 신호를 생성하여 설정합니다.

메세지에 들어갈 모든 정보를 입력한 후 ‘Spy Networks’에서 ‘Tx Panel’로 이동합니다. 이 창은 메세지를 송신하는 창으로 ‘Message Editor’ 창에서와 동일하게 ‘Description’과 ‘ArbID’의 값을 수정할 수 있으며 ‘B1’-’B8’의 항목에 직접 숫자를 입력할 수도 있습니다. 먼저 ‘Online’상태에서 원하는 메세지의 ‘Tx’항목에 있는 버튼을 누르게 되면 메세지가 보내지게 됩니다. 즉, 버튼을 한번 누를 때마다 한번씩 메세지가 보내지게 됩니다.

버튼을 눌렀을 때 특정 주기로 메세지가 보내지도록 설정 하고자 한다면 ‘Auto Tx’항목에 기본으로 설정되어 있는 ‘Periodic’을 ‘Periodic On/Off’로 바꾼 다음 ‘Rate’항목에 ‘None’으로 되어있는 곳에 원하는 주기 값(초)을 입력해줍니다. 그러면 ‘Online’한 후 ‘Tx’버튼을 누르게 되면 버튼이 눌려진 형태로 계속 유지가 되면서 설정한 주기마다 메세지가 나가게 됩니다.

또한 해당 메세지의 신호 값들은 ‘Tx Panel’의 오른쪽에 ‘Signals’항목에 보여지게 되고 아래와 같이 ‘Value’값에 직접 입력하거나 ‘In’(+)와 ‘Dc’(-)버튼을 이용하여 Step에 값만큼 증가시키거나 감소시킬 수 있습니다.
 
![Tx panel](img/TxPanel.png)

그리고 ‘Sg’의 항목을 이용하여 특정 주기로 된 신호를 보내실 수도 있습니다.
(위에서 보시면 현재 ‘Periodic On/Off’로 선택되어 있고 주기가’0.01’초로 설정되어 있습니다.)



여기에서 편리하게 사용하기 위해 두 가지 창을 동시에 보는 방법은 원하는 창의 이름 부분을 마우스로 클릭한 상태에서 원하는 쪽으로 이동하면 됩니다.
 
![Tx panel2](img/TxPanel2.png)

위와 같이 하면 아래 그림처럼 ‘Messages’ 창과 ‘Tx Panel’ 창을 한 화면에서 사용할 수 있습니다.
 
![Txpanel+Messages](img/Txpanel+Messages.png)
 
<div style="page-break-after: always;"></div>

## 4.3. 메세지 데이터 저장 파일 송신(Playback)

메세지 데이터를 저장한 파일(*.csv, *.vsb, *.snp, *.log, *.asc, *txt, *.dat, *.img, *.blf)을 저장 된 메세지의 순서대로 저희 장비에서 송신메세지를 보내주는 방법을 소개합니다. 즉, 실제 차량의 데이터를 사용하게 되면 차량에 연결 된 것과 동일한 메세지를 개발중인 장비로 보내어 테스트할 수 있습니다.

먼저 ‘Scripting and Automation’에서 ‘Function Blocks’로 이동합니다. 이동 후 ‘+’버튼을 누르고 ‘Playback’을 선택합니다. 그러면 Function Block이 생성되면서 Type에 ‘Playback’으로 표시됩니다. 그리고 아래 부분에 있는 ‘buffer’라는 항목에 ‘Browse…’버튼을 눌러 메세지 데이터를 저장한 파일을 등록해 줍니다. 그리고 시작을 어떻게 할 것인지 설정을 할 ‘Start’ 항목으로 이동합니다. 그러면 기본적으로 아래와 같이 ‘Start Immediately’로 설정되어 있습니다.
 
![Capture-Start](img/Capture-Start.png)

각 항목이 의미하는 바는 다음과 같습니다.
 - Start Immediately: Online과 동시에 등록한 데이터파일 메세지가 전송되는 방식
 - Manual Start: 내가 직접 시작하는 시점과 끝나는 시점을 정하는 방식
 - Use Start Expression: 아래와 같이 특정 수식이 참이 되었을 때 동작하는 방식

 ![Capture-StartExpression](img/Capture-StartExpression.png)


- Start Immediately Embedded Only: 장비에 직접 이 Function Block을 넣은 후 장비에서만 전원이 들어 왔을 때 바로 동작하는 방식(PC에서는 동작하지 않음)
‘Manual Start’에서 직접 동작을 시키는 방법에는 아래처럼 시작 버튼과 멈추는 버튼을 눌러서 직접 제어할 수 있고 ‘Start/Stop Hotkey’를 이용하여 해당 키를 눌러서 제어하거나 ‘Graphical Panels’에서 제어하는 방법이 있습니다.
 
![FunctionBlocks-Playback](img/FunctionBlocks-Playback.png)

그래서 Playback Function Block이 실행이 되면 ‘Running’항목이 위의 그림처럼 ‘Running’으로 표시가 되고 ‘Messages’ 창에서 보면 아래와 같이 메세지들이 송신되고 있는 것을 확인하실 수 있습니다.
 
![Messages-Playback](img/Messages-Playback.png)

<div style="page-break-after: always;"></div>

# 5. 진단 통신(UDS/CCP/XCP)

## 5.1. 진단용 데이터베이스 설정

### 5.1.1. ISO14229(UDS) 데이터베이스 등록

ISO14229(UDS) 진단 통신을 통해 차량의 VIN, DTC, DID, PID 등의 정보를 읽거나 변경할 수 있습니다. 이 통신을 하기 위해서는 ODX, CDD 등의 진단 데이터베이스 파일 또는 관련 스펙(진단 ID, 진단 서비스 ID 등)이 필요합니다. 경우에 따라 Security Access용 dll 파일이 추가로 필요합니다.

1. [데이터베이스 플랫폼을 생성](#12-데이터베이스-플랫폼-생성-및-데이터베이스dbc-ldf-arxml-등록)하거나 상단 바의 Platform 드롭다운 메뉴에서 기존의 플랫폼을 지정합니다.
2. 상단 메뉴 바의 ![](img/2022-02-03-14-40-06.png)를 누르거나 Spy Networks->ECUs 메뉴로 이동합니다.
3. 진단용 데이터베이스 파일이 있는 경우 메뉴 상단의 Import->ISO14229 (UDS)에서 가지고 있는 파일(ODX, CDD 등)을 등록합니다.
4. 좌측에 등록된 제어기 목록이 표시됩니다. Security Access가 필요한 제어기인 경우 좌측에서 ECU 선택, Security 탭에서 Browse...버튼을 눌러 dll 파일을 등록하고 Level과 Seed Size/Key Size를 설정합니다. ![](img/2022-01-07-11-06-15.png)
5. 파일 등록이 끝났으면 빨간색 박스가 깜빡 거리는 ![](img/2022-01-04-16-24-53.png) 버튼 또는 ![](img/2022-01-04-16-25-23.png)를 눌러 플랫폼 설정을 저장합니다.

### 5.1.2. CCP/XCP 데이터베이스 등록
CAN Calibration Protocol(CCP) 또는 Universal Calibration Protocol(XCP) 진단 통신을 통해 차량 메모리 변수 값을 읽고 로깅할 수 있습니다. 이 통신을 하기 위해서는 A2L 파일이 반드시 필요하며 경우에 따라 Security Access용 dll 파일이 추가로 필요합니다.

1. [데이터베이스 플랫폼을 생성](#12-데이터베이스-플랫폼-생성-및-데이터베이스-파일dbc-ldf-arxml-등록)하거나 상단 바의 Platform 드롭다운 메뉴에서 기존의 플랫폼을 지정합니다.
2. Mesurement->MEP 메뉴 왼쪽 상단의 ![](img/2022-01-06-17-20-02.png)를 클릭, Add for Measurement / Logging을 클릭하여 A2L 파일을 등록합니다.
3. 좌측에 등록된 제어기 목록이 표시됩니다. Security Access가 필요한 제어기인 경우 좌측에서 ECU 선택, Security 탭에서 Browse...버튼을 눌러 dll 파일을 등록합니다. 장비 단독 로깅을 할 때에는 Send To Device 버튼을 눌러 dll 파일을 장비에 심어줍니다. ![](img/2022-01-07-11-42-36.png)
4. 파일 등록이 끝났으면 빨간색 박스가 깜빡 거리는 ![](img/2022-01-04-16-24-53.png) 버튼 또는 ![](img/2022-01-04-16-25-23.png)를 눌러 플랫폼 설정을 저장합니다.

<div style="page-break-after: always;"></div>

## 5.2. 진단 통신 변수 모니터링

Vehicle Spy는 진단 통신 변수를 주기적으로 취득할 수 있도록 도와줍니다.

1. Measurement->Vehicle Scape DAQ로 이동합니다. 또는 아래의 File->Logon 화면에서 VehicleScape DAQ 버튼을 클릭합니다.

![Logon-VehicleScapeDAQ](img/Logon-VehicleScapeDAQ.png)]

2. Channels 탭에서 읽을 변수를 추가합니다. Clear 버튼을 누르면 하단 Results 창에 현재 등록된 플랫폼 내의 모든 변수가 출력됩니다. 또는 검색된 변수의 목록이 출력됩니다. 로깅을 원하는 변수를 더블 클릭 또는 드래그로 다중 선택하여 Selected>> 버튼을 누르면 변수들이 우측 Selected Channels for Test에 추가됩니다. 

3. 상단의 Polling setup에서 변수 취득 주기를 설정하고 변수들을 우클릭하여 Rate를 Low/Normal/High 중 하나로 선택합니다. CCP/XCP 변수를 Event 방식으로 받는 경우 변수들을 우클릭 후 Rate->CCP/XCP DAQ Events에서 Event를 지정합니다. Event별로 할당할 수 있는 ODT 갯수가 정해져있으므로 메뉴 우측 하단의 표를 참고하여 이를 초과하지 않도록 지정합니다.

![](img/2022-01-07-14-43-25.png)

4. Online 탭으로 이동하면 변수 값이 표시됩니다. 변수 값이 나오지 않은 경우 (Re)start 버튼을 누릅니다.

![](img/2022-01-07-15-08-21.png)

이어서 장비 단독 변수 로깅은 [여기](#24-장비-단독으로-메세지-저장법)를 참고하시기 바랍니다.

<div style="page-break-after: always;"></div>

## 5.3. Diagnostics 메뉴를 이용한 UDS 진단

5.2와 같은 방법이 아니라 개별적으로 UDS 진단 Request를 수행하고 싶을 때에는 아래 절차를 따르면 됩니다.

1. Spy Networks->Diagnostics 메뉴로 이동합니다.
2. 등록한 데이터베이스 파일 내에 진단 수행에 대한 정보가 있으면 좌측에 Database Jobs 목록에 표시됩니다. 원하는 진단의 체크 박스를 클릭하여 진단을 수행하면 상단에 진단 결과가 표시됩니다. ![](img/2022-01-06-17-40-48.png)


<div style="page-break-after: always;"></div>

# 6. 자주 묻는 질문(FAQ)

## 6.1. DBC 파일을 편집하는 방법

Vehicle Spy를 통해 가지고 계신 DBC의 정보를 수정 후 새로운 dbc 파일로 저장할 수 있습니다. 

1. 수정하고자 하는 DBC 파일을 등록합니다. DBC 파일 등록법은 [여기](#12-데이터베이스-플랫폼-생성-및-데이터베이스dbc-ldf-arxml-등록)에 소개되어있습니다.

2.	Spy Networks->Messages Editor 메뉴의 Database 탭에서 등록한 DBC에 정의된 내용을 확인할 수 있습니다. 그러나 아래 그림과 같이 수정할 수 없도록 Edit Signal 창의 OK 버튼이 비활성화되어 있습니다. 
 
![MessagesEditor-Database](img/MessagesEditor-Database.png)

3.	Shift+클릭을 이용해 데이터 베이스 메세지를 전체 선택 한 후 마우스 우클릭 Copy To Receive를 선택합니다.

![CopyToReceive](img/2021-10-14-10-26-34.png)

4. Receive 탭으로 이동 후 복제된 메세지들을 원하시는 대로 수정합니다. 수정 방법은 [여기](#41-수신-메세지-생성-및-dbc-파일-생성)를 참고하시기 바랍니다.  
 
![MessagesEditor-Receive](img/2021-10-14-10-31-12.png)

5. 수정이 끝난 후 Messages Editor 메뉴 상단의 ![MessagesEditor-ExportDatabase](img/2021-10-14-10-33-10.png) 버튼을 누른 뒤 새로운 DBC 파일로 저장합니다.

<div style="page-break-after: always;"></div>

## 6.2. Logging 데이터 통합/분할/맵핑 (VSB Editor)

Vspy3를 통해 로깅한 파일(.vsb)의 데이터 용량이 큰 경우, 분석하는데 불편함을 초래할 수 있습니다. 반대로, 데이터가 여러 파일로 분산된 경우 분석하는데 용이하지 않습니다. 이런 경우, Vspy3의 VSB Editor를 이용해 파일을 Combine/Split 할 수 있습니다. 방법은 다음과 같습니다. 
a.	Tools > File Conversions > VSB Editor클릭
 
b.	Split/Combine tab 선택 후, Select Path를 이용해 작업을 수행할 VSB를 선택 및 
Split/Combine button 클릭

![VSBEditor-SplitVSB](img/VSBEditor-SplitVSB.png)

추가적으로, VSB Editor에서는 맵핑(Mapping)이라는 기능을 제공하고 있습니다. 로깅한 파일의 차량 네트워크를 사용자의 환경에 맞게 다시 맵핑(Remapping)할 수 있는 기능입니다. VSB Editor의 Remap VSB를 통해 네트워크를 수정할 수 있습니다. 

1. Select Path클릭, 수정할 VSB 선택
2. Scan VSB 클릭하여 내용 불러오기
3. To tab의 네트워크 더블 클릭 후, 수정
4. Remap VSB 클릭하여 변경 내용 적용

![VSBEditor-RemapVSB](img/VSBEditor-RemapVSB.png)

<div style="page-break-after: always;"></div>

## 6.3. VSB 파일 변환 방법

Vehicle Spy Binary(VSB) 파일은 Vehicle Spy 자체 로그 파일 형식입니다. vsb 파일은 시그널과 같은 데이터베이스 정보는 포함되어있지 않습니다. 필요하신 경우 다른 파일 포맷으로 변환할 수 있습니다.

### 6.3.1. VSB에서 .csv, .asc, .blf 등의 포맷으로 변환 

Tools->File Conversions에서 아래와 같이 csv, asc, blf 등의 파일 변환 기능을 제공하고 있습니다.
 ![File Conversions](img/2022-02-28-10-09-31.png)

### 6.3.2. VSB에서 MDF(.dat, .mdf, .mf4) 포맷으로 변환

mdf 파일은 시그널 형식의 파일로 vsb 파일을 mdf 파일로 변환하기 위해서는 Vehicle Spy 데이터베이스 형식인 vsdb 파일이 필요합니다.

vsdb 파일을 생성하는 방법은 다음과 같습니다.

- PC 없이 장비 단독으로 로깅하신 경우: 
  장비에서 로그파일을 추출하면 vsdb 파일이 로그 파일(vsb)과 함께 추출됩니다.
- PC에서 로깅 하셨거나, vsb 파일만 단독으로 가지고 계신 경우: 
  아래 방법으로 vsdb 파일을 생성합니다.
 1. [1.2. 데이터베이스 플랫폼 생성 및 데이터베이스(.dbc, .ldf, .arxml) 등록](#12-데이터베이스-플랫폼-생성-및-데이터베이스dbc-ldf-arxml-등록)을 참고하여 데이터 베이스를 등록합니다. 이때 로그 파일 상의 채널 번호와 데이터베이스 상의 채널 번호가 일치하는지 확인합니다.
 2. Measurement->Vehiclescape DAQ->Standalone Logging 탭에서 설정 변경 없이 하단의 Generate 버튼을 누릅니다. CoreMini Executable Generator 창이 뜨면 아무 것도 누르지 않고 다시 닫습니다.
 3. 오른쪽 상단의 ![Data](img/2022-02-03-15-04-05.png)를 누르면 DAQ 1.vsdb 파일이 생성되는 경로가 열립니다.

변환하는 방법은 다음과 같습니다.

1. 변환할 파일(vsb)가 있는 폴더에 앞서 만든 DAQ 1.vsdb 파일을 복사합니다.
2. Tools->Extract/Export에서 Export탭으로 이동합니다.
3. Output 경로 옆 Browse...버튼을 눌러 변환할 파일(vsb)이 있는 경로를 선택합니다.
4. 화면 우측에 데이터베이스내 시그널 목록이 표시되며 로그 파일 안에 존재하는 시그널이 모두 자동으로 체크됩니다. 일부 시그널만 추출할 경우 추출을 원하는 시그널만 선택합니다.
5. 왼쪽 하단 Signal Data 드롭다운에서 MDF체크 후 Export를 누르면 변환됩니다. 기본 .dat 파일로 추출되며 오른쪽 상단 Advanced  Settings...->Export탭에서 .mdf, .mf4 등으로 변경 가능합니다.
![](img/2022-02-28-13-13-23.png)

<div style="page-break-after: always;"></div>

## 6.4. neoVI FIRE2를 이용한 아날로그 값 측정법(eMISC 사용법)

아날로그 값 측정은 FIRE2 장비의 마이크로 9핀을 이용합니다. 8/9번 두 채널이 있으며 5번이 그라운드입니다. 측정 가능한 범위는 0~40V이며 resolution은 12bit입니다. 

![](img/2021-11-15-15-07-25.png)
![](img/2021-11-15-15-08-43.png)

FIRE2 장비 설정은 다음과 같이합니다.

Vehicle Spy 상단 메뉴바 ![NeoVi Explorer icon](img/2020-01-02-11-31-14.png) 클릭 > 좌측에서 장비 선택 후 Connect 클릭 > MISC IO와 Initial Values 옵션을 다음과 같이 설정 > Write Settings 클릭

![](img/2021-11-17-11-11-40.png)
![](img/2021-11-17-11-12-37.png)

이후 시그널 값은 neoVI 채널(HS CAN 채널 X)의 Report Messages 메세지 안의 EMISC1 AIN, EMISC2 AIN 시그널로 수신됩니다.

![](img/2021-11-17-11-15-00.png)

<div style="page-break-after: always;"></div>

## 6.5. 케이블별 핀맵

[여기](http://www.intrepidcs.co.kr/uploads/2/5/0/1/25016645/icsk_%EC%BC%80%EC%9D%B4%EB%B8%94%EB%B3%84_%ED%95%80%EB%A7%B5.pdf)를 눌러 케이블별 핀맵을 확인하실 수 있습니다.

<div style="page-break-after: always;"></div>

## 6.6. Vehicle Spy 퍼포먼스 개선 옵션

저사양 PC에서 Vehicle Spy를 구동하시거나, Tx panel을 이용하여 메세지 송신시 설정한 주기보다 송신 되는 메세지 주기가 길어지는 경우 다음과 같은 방법으로 소프트웨어 퍼포먼스를 개선하실 수 있습니다. 


1. Tools->Options에서 아래와 같이 Core loop 시간을 1ms로 조정해주세요.

![img](img/Options-Performance.png)

추가적으로 속도 향상을 원하시면 아래 옵션을 추가로 변경해주세요. 
(이 추가 옵션은 vehicle spy를 두 개 이상 실행시에는 효과가 없습니다.)

2. Tools->Options의 Performance탭에서 Core loop 글자를 더블 클릭하시면 아래와 같은 창이 뜹니다. 
Affinity 설정을 통해 Vehicle Spy 각 기능마다 어떤 CPU 코어를 쓸지 할당 할 수 있습니다. 예를 들어 인텔사 듀얼코어는 0,2번이 실제 코어이고 1,3번은 hyperthread입니다. 이 경우 GUI와 Core에 같은 코어(0)를 그리고 Hardware Rx와 Hardware TX에 같은 코어(2)를 할당하시는 것을 추천드립니다. 인텔사 쿼드코어를 사용 중이시라면 각각에 0,2,4,6번 코어를 할당하시면 됩니다. 

![img](img/Options-Performance2.png)

<div style="page-break-after: always;"></div>

감사합니다!
사용법에 관한 문의는 아래 연락처로 주시기 바랍니다.

<a name="contacts"></a> Contacts <br>
Tel: 070-4680-3601<br>
e-mail: icskoreasupport@intrepidcs.com
 

[온라인 동영상 강의](https://www.intrepidcs.co.kr/vspy-video-guide.html)를 통해 Vspy3의 기초 사용법 및 더 강력한 고급기능을 배워볼 수 있습니다.


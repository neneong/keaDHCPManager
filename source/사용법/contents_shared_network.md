Shared Network
=====================
    url: /shared_network
네비게이션 바에서 **shared network**을 클릭해 shared network 페이지를 열 수 있다.  

shared network 생성하기
--------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2017.10.52.png?raw=true)

우측 상단 빨간색 **CREATE**버튼을 클릭해 subnet 생성 폼을 띄울 수 있다.  
띄워진 subnet 생성 폼에서 **ip version**, **Server**를 선택할 수 있으며 **shared network name**를 입력할 수 있다.
원하는 정보를 입력한 후 **Submit**버튼을 클릭하여 shared network를 생성할 수 있다.  

kea dhcp server의 상세페이지에서 **Create Shared Network**버튼을 클릭하여 kea dhcp server의 정보가 미리 선택되어 있는 상태로 shared network 생성이 가능하다.  

shared network 모니터링
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2017.25.05.png?raw=true)
shared network 페이지에서 생성 되어있는 shared network의 정보를 일정시간마다 업데이트 되는 정보를 모니터링 할 수 있다. 또한 우측 상단 검색 기능을 이용하여 원하는 정보들만 모아 볼 수 있다.   

shared network 상세정보
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2017.30.33.png?raw=true)
shared network페이지에서 shared network 주소를 클릭하여 상세 페이지를 열 수 있다.   
shared network의 상세페이지에선 shared network의 설정을 수정하거나, subnet 정보를 생성, 다른 subnet을 해당 shared network에 포함 시킬 수 있고 shared network를 삭제할 수 있다.  

shared network 설정
-------------------
### IP 할당 전략
shared network 상세 페이지에서 **IP 할당 전략**을 이용하여 **다음에 생성될** 하위 shared network와 subnet의 ip 할당 전략을 변경할 수 있다.  
IP 할당 전략의 **콤보 박스**에서 원하는 할당 전략을 선택하고 **update**버튼을 눌러 할당 전략을 변경할 수 있다.  

shared network 삭제
-------------------
shared network 상세페이지의 Settings 마지막에 있는 **DELETE THIS SHARED NETWORK**를 이용하여 shared network을 삭제할 수 있다.  
shared network 삭제시 삭제한 shared network에 등록 되어 있는 subnet이 삭제된다.  
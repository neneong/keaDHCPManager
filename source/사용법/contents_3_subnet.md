Subnet
=====================
    url: /subnet
네비게이션 바에서 **subnet**을 클릭해 subnet 페이지를 열 수 있다.  

subnet 생성하기
--------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2016.31.41.png?raw=true)

우측 상단 빨간색 **CREATE**버튼을 클릭해 subnet 생성 폼을 띄울 수 있다.  
띄워진 subnet 생성 폼에서 **ip version**, **Server**, **Shared Network**, **Subnet Mask**를 선택할 수 있다. 
또한 **Ip Address**를 입력할 수 있으며, 올바른 정보를 입력하면 입력한 서브넷 주소의 Subnet Range, Network Address, Broadcast Address, Total Host Address Count를 함께 볼 수 있다.  
원하는 정보를 입력한 후 **Submit**버튼을 클릭하여 subnet을 생성할 수 있다.  
subnet이 생성되면 subnet 전체 범위와 같은 범위를 가진 pool이 자동으로 생성된다.

kea dhcp server의 상세페이지, shared network의 상세페이지에서 **Create Subnet**버튼을 클릭하여 kea dhcp server의 정보나 shared network의 정보가 미리 선택되어 있는 상태로 subnet 생성이 가능하다.  

subnet 모니터링
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2016.50.48.png?raw=true)
subnet 페이지에서 생성 되어있는 subnet의 정보를 일정시간마다 업데이트 되는 정보를 모니터링 할 수 있다. 또한 우측 상단 검색 기능을 이용하여 원하는 정보들만 모아 볼 수 있다.   

subnet 상세정보
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2016.54.59.png?raw=true)
subnet페이지에서 subnet 주소를 클릭하여 상세 페이지를 열 수 있다.   
subnet의 상세페이지에선 subnet의 설정을 수정하거나, pool이나 reservation 정보를 추가, subnet을 삭제할 수 있다.  

subnet 설정
-------------------

### IP 할당 전략
subnet 상세 페이지에서 Settings의 **IP 할당 전략**을 이용하여 subnet에 적용될 ip 할당전략을 변경할 수 있다.  
IP 할당 전략의 **콤보 박스**에서 원하는 할당 전략을 선택하고 **update**버튼을 눌러 할당 전략을 변경할 수 있다.

### subnet이 소속된 shared network
subnet 상세 페이지에서 Settings의 **shared network**을 이용하여 subnet이 소속된 shared network를 변경하거나 소속되지 않게 할 수 있다.

subnet 삭제
-------------------
subnet 상세페이지의 Settings 마지막에 있는 **DELETE THIS SUBNET**를 이용하여 subnet을 삭제할 수 있다.  
subnet 삭제시 삭제한 subnet에 등록 되어 있는 pool이 삭제된다.  
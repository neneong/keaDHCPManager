Kea DHCP Server
=====================
    url: /kea
네비게이션 바에서 **kea server**를 클릭해 kea server 페이지를 열 수 있다.  

kea dhcp server 추가하기
--------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2015.13.02.png?raw=true)

우측 상단 빨간색 **ADD**버튼을 클릭해 원하는 이름과 서버의 주소를 입력할 수 있다. 
원하는 정보를 입력한 후 **Submit**버튼을 클릭하여 원하는 서버를 추가할 수 있다.  

kea dhcp server 모니터링
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2016.27.46.png?raw=true)
kea server 페이지에서 추가되어있는 kea dhcp server들의 일정시간마다 업데이트 되는 정보를 모니터링 할 수 있다. 또한 우측 상단 검색 기능을 이용하여 원하는 정보들만 모아 볼 수 있다. 

kea dhcp server 상세정보
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2016.07.21.png?raw=true)  
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-07%2016.15.49.png?raw=true)
kea server 페이지에서 kea dhcp server의 이름을 클릭하여 상세 페이지를 열 수 있다.  
kea dhcp server의 상세페이지에선 kea dhcp server의 설정을 수정하거나, subnet이나 shared network를 추가, kea dhcp server를 삭제할 수 있다.

kea dhcp server 설정
-------------------
kea dhcp server의 설정은 대부분 DHCP4 서버와 DHCP6 서버의 설정을 따로 관리한다.  
또한 

### 임대 정보 데이터베이스 설정
kea server 상세페이지에서 **DHCP4 데이터베이스 설정** 또는 **DHCP6 데이터베이스 설정**을 이용하여 임대 정보를 저장할 데이터베이스를 설정할 수 있다.  
DHCP4 데이터베이스 설정 또는 DHCP6 데이터베이스 설정의 **update**버튼을 클릭하여 임대 정보 데이터베이스 설정 폼을 띄울 수 있다.  

### 만료된 임대 정보 처리(임대 정보 회수 처리) 설정
kea server 상세페이지에서 **DHCP4 만료된 임대 정보 처리** 또는 **DHCP6 만료된 임대 정보 처리**를 이용하여 임대 정보를 회수하기 위한 설정을 할 수 있다.  
DHCP4 만료된 임대 정보 처리 또는 DHCP6 만료된 임대 정보 처리의 **update**버튼을 클릭하여 임대 회수 절차를 수정할 수 있는 폼을 띄울 수 있다.  

임대 회수 절차에 대한 자세한 내용은 [kea 공식문서][https://kea.readthedocs.io/en/kea-2.4.0/arm/lease-expiration.html]를 참고하십시오.

### IP 할당 전략
kea server 상세 페이지에서 **DHCP4 IP 할당 전략** 또는 **DHCP6 IP 할당 전략**을 이용하여 **다음에 생성될** 하위 shared network와 subnet의 ip 할당 전략을 변경할 수 있다.  
DHCP4 IP 할당 전략 또는 DHCP6 IP 할당 전략의 **콤보 박스**에서 원하는 할당 전략을 선택하고 **update**버튼을 눌러 할당 전략을 변경할 수 있다.  

DHCP6 서버의 IP 할당 전략은 FLQ를 사용할 수 없다. 

DHCP6 서버의 IP 할당 전략으로 FLQ를 사용할 수 없는 자세한 이유는 [kea 공식문서][https://kea.readthedocs.io/en/kea-2.4.0/arm/lease-expiration.html]를 참고하십시오.
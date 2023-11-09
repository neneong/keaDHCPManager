Pool
=====================
    url: /pool
네비게이션 바에서 **pool**을 클릭해 pool 페이지를 열 수 있다.  

pool 생성하기
--------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-08%2010.00.11.png?raw=true)

우측 상단 빨간색 **Add Pool**버튼을 클릭해 pool 추가 폼을 띄울 수 있다.  
띄워진 pool 추가 폼에서 **Subnet**과 **ip version**, **Server**를 선택할 수 있다.  
또한 **Pool Range**를 입력할 수 있다. 다른 pool과 범위가 겹치거나, 서브넷의 범위를 벗어나면 안 된다.  
일반적인 경우 subnet 생성시에 자동으로 생성된 pool의 범위를 수정 하거나 삭제 후 pool을 추가해야한다.  
원하는 정보를 입력한 후 **Submit**버튼을 클릭하여 subnet을 생성할 수 있다.  

subnet의 상세페이지에서 **Add Pool**버튼을 클릭하여 kea dhcp server 정보, subnet 정보가 미리 선택되어 있는 상태로 pool 생성이 가능하다.  

pool 모니터링
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-08%2010.36.20.png?raw=true)
pool 페이지에서 생성 되어있는 pool의 사용량을 일정시간마다 업데이트 되는 정보를 모니터링 할 수 있다.

pool 상세정보
-------------------
![사진을 불러올 수 없습니다.](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202023-11-08%2010.39.16.png?raw=true)
pool페이지에서 pool 주소를 클릭하여 상세 페이지를 열 수 있다.   
pool의 상세페이지에선 pool의 범위나 설정을 수정하거나, reservation 정보를 추가, lease 정보를 강제 삽입, pool을 삭제할 수 있다.  

pool 삭제
-------------------
pool 상세페이지의 Settings 마지막에 있는 **DELETE THIS POOL**를 이용하여 pool을 삭제할 수 있다.  
pool 삭제시 삭제한 pool에 등록 되어 있는 임대 정보가 삭제될 수 있으며 삭제된 pool의 범위는 다른 pool을 생성하거나 기존 pool의 범위를 수정 할 때 사용될 수 있다.
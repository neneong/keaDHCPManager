kea DHCP Manager 설치 방법
============

kea DHCP Manager는 java spring boot 기반의 애플리케이션으로, 
기본적으로 실행하기 위해서는 java 17 이상 버전이 설치되어 있어야 합니다.
또한, kea가 설치되어있어야 하며 여기에서는 기본적인 kea 설치 및 java 환경까지 설정을 마쳤다는 전제 하에 설명하도록 하겠습니다.

저희가 드린 kea-dhcp-manager.jar 파일을 다음과 같이 실행합니다.

`java -jar kea-dhcp-manager.jar`

![사진을 불러올 수 없습니다](https://github.com/neneong/keaDHCPManager/blob/main/source/_static/start-spring-boot.png?raw=true)

만약 실행이 정상적으로 되지 않는다면 다음의 항목을 체크해주세요.

1. 서버의 8080 포트를 사용하는 프로그램이 있는가?
2. 서버의 java 버전이 17 이상인가?
3. 서버에 파일을 넣고 권한을 제대로 주었는가?


실행이 정상적으로 되었다면, 서버 아이피 주소:8080으로 접속해주세요

예시 : 
`192.168.0.2:8080`

만약 접속이 되지 않는다면 다음 항목을 체크해보세요.

1. 서버의 8080 포트가 열려있는가?
2. 정상적으로 서버 파일이 실행되었는가?

만약 위의 항목을 체크하였는데도 접속이 되지 않는다면, aaa@example.com으로 연락주시기 바랍니다.
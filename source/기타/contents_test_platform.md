테스트된 플랫폼
============


현재 kea DHCP MANAGER가 테스트된 환경은 다음과 같습니다.

+ iptime N704BCM 라우터(펌웨어 12.16.2)
    + dhcp 서버 설정 : 중지
    + 내부 네트워크 설정
        + 내부 아이피 주소 : 192.168.0.1
        + 서브넷 마스크 255.0.0.0

<br>

+ kea 서버 환경
    + debian 12
    + java 17 설치환경
    + 무선랜, 유선랜 연결
        + 유선랜은 bridge로 연결 후, 수동으로 ip 구성(192.168.0.233)

<br>

+ kea dhcp manager 환경
    + macOS 13
    + java 17 설치환경
    + 맥북에 유선랜 추가로 연결된 환경
    + 서버 아이피는 192.168.0.7로 고정
<br>

+ kea dhcp manager 환경(프론트엔드)
    + macOS 13
    + nodejs 20.5.1
    + vite, storybook 설치 환경


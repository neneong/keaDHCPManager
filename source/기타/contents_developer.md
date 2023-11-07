개발자를 위한 문서
===============

개발 도움 문서
-------------

kea DHCP MANAGER에서는 기본적으로 swagger api 문서를 제공합니다.
서버 주소:8080 /swagger-ui/index.html에 들어가면 보실 수 있습니다.

`http://서버주소:8080/swagger-ui/index.html`

크게 dhcp4, dhcp6, event, keaCtrl, lease, member, pinned, pool4, pool6, server,
serverConfigs, subnet4, subnet6 등으로 나뉘어 있습니다.

1. dhcp4
    dhcp의 ipv4 버전을 담당하는 api입니다.

2. dhcp6
    dhcp의 ipv6 버전을 담당하는 api입니다.

3. event
    서버에서 발생한 이벤트를 담당하는 api입니다

4. keaCtrl
    kea의 kea-ca를 담당하는 api입니다.

5. lease
    kea의 dhcp4, dhcp6 임대 통계를 담당하는 api입니다.

6. member
    kea management server의 사용자를 담당하는 api입니다.

7. pinned
    서버 대시보드에 핀을 담당하는 api입니다.

8. pool4
    임대 풀 중에서 ipv4 영역을 담당하는 api입니다.

9. pool6
    임대 풀 중에서 ipv6 영역을 담당하는 api입니다.

10. server
    kea 서버의 설정을 담당하는 api입니다.

11. serverConfigs
    kea 서버의 통합 설정(dhcp4, dhcp6, server)을 담당하는 api입니다.

12. subnet4
    서브넷 중에서 ipv4를 담당하는 api입니다.

13. subnet6
    서브넷 중에서 ipv6를 담당하는 api입니다.
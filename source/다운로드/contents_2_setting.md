kea DHCP Manager에 연결하기 위한 kea 설정
===============

kea DHCP Manager는 kea와의 연동을 위해 kea control agent를 사용합니다.
이를 사용하기 위해서는 일부 설정이 필요합니다.

기본적으로 kea control agent의 설정 파일은 기본적으로 다음의 경로에 위치해 있습니다.

`/usr/local/etc/kea/kea-ctrl-agent.conf`

해당 파일을 텍스트 편집기로 열어보면 다음과 같이 나옵니다.

`
{
  "Control-agent": {
    "control-sockets": {
      "d2": {
        "socket-name": "/tmp/kea-ddns-ctrl-socket",
        "socket-type": "unix"
      },
      "dhcp4": {
        "socket-name": "/tmp/kea4-ctrl-socket",
        "socket-type": "unix"
      },
      "dhcp6": {
        "socket-name": "/tmp/kea6-ctrl-socket",
        "socket-type": "unix"
      }
    },
    "hooks-libraries": [ ],
    "http-host": "127.0.0.1",
    "http-port": 8000,
    "loggers": [
      {
        "debuglevel": 0,
        "name": "kea-ctrl-agent",
        "output_options": [
          {
            "flush": true,
            "maxsize": 10240000,
            "maxver": 1,
            "output": "/usr/local/var/log/kea-ctrl-agent.log",
            "pattern": ""
          }
        ],
        "severity": "INFO"
      }
    ]
  }
}
`

여기에서 http-host를 바꾸어줘야 정상적으로 작동됩니다.

http-host를 127.0.0.1에서 서버 주소로 바꿔주세요.

바꾼 후, keactrl을 이용하여 정지 후, 시작 해주세요.

`
keactrl stop
keactrl start
`

아무 오류 없이 정상적으로 시작된다면 kea를 kea Manager 서버에 연결할 준비는 거의 끝났습니다.

만약 서버에 방화벽이 있다면, 8000포트를 열어주세요.

만약 이렇게 하였는데에도 연결이 안된다면 다음을 체크해주세요.

1. kea 서버와 kea Manager 서버가 같은 대역에 있는가?

2. kea 서버에 방화벽이 있는가? 그렇다면, 방화벽에서 8000 포트를 허용하였는가?

3. kea control agent 설정 파일에 문제가 있는가? 

만약 위의 항목을 체크하였는데도 접속이 되지 않는다면, aaa@example.com으로 연락주세요
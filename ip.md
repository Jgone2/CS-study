# IP(Internet Protocol)

- 지정한 IP 주소(IP Address)에 데이터를 전달
- 패킷(Packet)이라는 통신 단위로 데이터 전달

# IP 프로토콜의 한계

- 비연결성
  - 패킷을 받을 대상이 없거나 서비스 불능 상태여도 패킷 전송
- 비신뢰성
  - 중간에 패킷이 사라지면?
  - 패킷이 순서대로 안오면?
- 프로그램 구분
  - 같은 IP를 사용하는 서버에서 통신하는 애플리케이션이 둘 이상일 때 패킷 전달 순서에 문제가 발생

# TCP(Transmission Control Protocol)
- 연결지향(TCP 3 way handshake[가상 연결])
- 데이터 전달 보증
- 순서 보장
- 신뢰할 수 있는 프로토콜
- 현재는 대부분 TCP사용
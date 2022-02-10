# 1. 운영체제(Operating System)

운영체제는 컴퓨터 시스템의 각종 자원을 효율적으로 관리하고 컴퓨터 HW(CPU, I/O)와 User간의 인터페이스를 담당하는 시스템 프로그램이다.<br />

- 프로그램들이 자원을 필요로 할 때 할당함
- 각각 자원을 할당받은 프로그램들이 서로 엉키지 않도록 제어함
- 하드웨어(HW)와 사용자간의 인터페이스를 담당

운영체제의 종류로는 MacOS, Linux, Windows, Android, iOS가 대표적이다.
<br /><br />

## 01. 운영체제 부팅과정

운영체제 역시 소프트웨어(SW)이므로 컴퓨터의 전원이 켜지면 메모리에 운영체제를 적재한다. 이 과정에서 ROM에 저장되어 있는 `부트로더(Boot Loader)`에 의해서 적재된다.<br />
![운영체제 부팅과정](https://vividswan.github.io/assets/images/201101-2.png)<br />

1. 컴퓨터의 전원이 On 상태가 되면 `POST(Power-On Self Test)`를 실행하여 컴퓨터에 연결되어 있는 HW(I/O 등)의 연결 상태가 정상인지 확인
2. OS는 비휘발성 저장장치인 보조기억장치에 저장되어 있으므로, ROM의 부트로더를 통해서 보조기억장치에 있는 OS에 접근
3. 보조기억장치에 있는 OS를 RAM에 적재해서 실행
4. OS가 Processor에 관여하며, 컴퓨터가 종료될 때까지 RAM에 적재상태를 유지

> 💡 **부트로더(Boot Loader)**<br />
> 운영체제가 시동되기 이전에 미리 실행되어 커널이 올바르게 시동되기 위해 필요한 모든 관련 작업을 마무리하고, 최종적으로 운영체제를 시동시키기 위한 목적을 가진 프로그램

<br />

# 02. 운영체제의 역할

- 프로세스 관리(Process Management)
- 메모리 관리(Memory Management)
- 저장소 관리(Storage Management)
- 보안(Protection and Security)

<br />

# 2. 인터럽트(Interrupt)

인터럽트는 운영체제가 어떤 작업을 수행하고 있을 때, 하드웨어나 프로그램으로부터 받는 새로운 신호를 말한다. 사전적 의미처럼 `방해`의 의미로, 작업 수행 중 인터럽트 신호를 받게 되면 진행중인 작업을 일시 중단하고 인터럽트 신호에 포함된 작업을 먼저 수행하게 된다.

1. 인터럽트가 발생되면 OS는 다음에 실행할 명령어를 스택(stack)에 저장
2. 발생된 인터럽트를 수행
3. 인터럽트가 종료되면 스택에 저장된 명령어 주소로 돌아가서 다음 명령어를 수행하거나 대기상태 복귀

<br />

# 3. 운영체제 작동방식의 발전

DOS와 같은 초기의 운영체제는 하나의 CPU에서 하나의 프로그램만 실행되는 단일 프로그래밍 시스템에서 현재의 빠르고 효율적인 시스템의 운영체제로 발전되어왔다.<br />
**일괄처리 시스탬 - 다중프로그램 시스템 - 시분할처리 시스템 - 실시간처리 시스템 - 분산처리 시스템 - 병렬처리 시스템**

## 01. 일괄처리 시스템(Batch System)

![](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FdQp4a3%2Fbtq4F1ORZCJ%2FPuXBXMfVbR9KNjfDrajSkK%2Fimg.png)<br />

- 유사한 요구를 가지는 작업을 모아 하나의 그룹으로 수행하는 시스템
- 하나의 CPU로 하나의 작업만 처리 할 수 있어서, 하나의 작업이 끝날 때까지 다른 작업은 대기
- 효율성이 낮음

## 02. 다중 프로그램 시스템(Multi-Programmed System)

![](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fb34vKR%2Fbtq4Ec37UPv%2F7Ukxg6JqAQW7hUBwZRfon1%2Fimg.png)<br />

- 처리해야할 프로세스가 있을 시 수행할 작업을 항상 가지도록 하는 시스템
- A프로세스에서 입출력을 수행중일 때, B작업에 CPU를 할당해서 처리하는 방식
- A프로세스에 CPU를 할당해서 작업중인 경우, I/O 장치들을 대기 상태로 만들어서 입출력이 필요한 작업에게 입출력 리소스를 할당

# 📚 Reference

[ROM의 Boot Loader](https://vividswan.github.io/2020/11/01/%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C-ROM%EC%9D%98-Boot-Loader.html)<br />
[운영체제의 구조와 원리](https://velog.io/@brian_kim/OS-%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C-%EA%B5%AC%EC%A1%B0%EC%99%80-%EC%9B%90%EB%A6%AC)<br />
[OS의 기본적인 작동 방식](https://choirim.tistory.com/65)<br />

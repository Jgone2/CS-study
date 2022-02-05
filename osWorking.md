# 1. 운영체제(Operating System)

운영체제는 컴퓨터 시스템의 각종 자원을 효율적으로 관리하고 컴퓨터 HW(CPU, I/O)와 User간의 인터페이스를 담당하는 시스템 프로그램이다.<br />

- 프로그램들이 자원을 필요로 할 때 할당함
- 각각 자원을 할당받은 프로그램들이 서로 엉키지 않도록 제어함
- 하드웨어(HW)와 사용자간의 인터페이스를 담당

운영체제의 종류로는 MacOS, Linux, Windows, Android, iOS가 대표적이다.
<br /><br />

# 2. 운영체제 부팅과정

운영체제 역시 소프트웨어(SW)이므로 컴퓨터의 전원이 켜지면 메모리에 운영체제를 적재한다. 이 과정에서 ROM에 저장되어 있는 `부트로더(Boot Loader)`에 의해서 적재된다.<br />
![운영체제 부팅과정](https://vividswan.github.io/assets/images/201101-2.png)<br />

1. 컴퓨터의 전원이 On 상태가 되면 `POST(Power-On Self Test)`를 실행하여 컴퓨터에 연결되어 있는 HW(I/O 등)의 연결 상태가 정상인지 확인
2. OS는 비휘발성 저장장치인 보조기억장치에 저장되어 있으므로, ROM의 부트로더를 통해서 보조기억장치에 있는 OS에 접근
3. 보조기억장치에 있는 OS를 RAM에 적재해서 실행
4. OS가 Processor에 관여하며, 컴퓨터가 종료될 때까지 RAM에 적재상태를 유지

> 💡 **부트로더(Boot Loader)**<br />
> 운영체제가 시동되기 이전에 미리 실행되어 커널이 올바르게 시동되기 위해 필요한 모든 관련 작업을 마무리하고, 최종적으로 운영체제를 시동시키기 위한 목적을 가진 프로그램

<br />

# 3. 운영체제의 역할

- 프로세스 관리(Process Management)
- 메모리 관리(Memory Management)
- 저장소 관리(Storage Management)
- 보안(Protection and Security)

# 📚 Reference

[ROM의 Boot Loader](https://vividswan.github.io/2020/11/01/%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C-ROM%EC%9D%98-Boot-Loader.html)<br />
[운영체제의 구조와 원리](https://velog.io/@brian_kim/OS-%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C-%EA%B5%AC%EC%A1%B0%EC%99%80-%EC%9B%90%EB%A6%AC)<br />
[OS의 기본적인 작동 방식](https://choirim.tistory.com/65)<br />

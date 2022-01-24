# 1. 터미널(Terminal)

- 터미널은 원래 UNIX기반의 대형 컴퓨터에서 사용자들이 컴퓨터에 접속하기 위해 사용했던 단말기를 의미(현재, 소프트웨어형태로 제공)
- 컴퓨터는 지금과 같은 GUI(Graphical User Interface)가 보편화되기 이전에는 터미널을 통해 컴퓨터를 조작하는 CLI(Command Line Interface)를 주로 사용
- GUI환경의 개발 도구에서도 모든 기능이 지원되지만 CLI로 작업 시 더 신속하고 편리하기 때문에 CLI에 익숙해 져야 함
>💡 CLI는 화면상에서 마우스 등을 이용해 컴퓨터를 조작하는 것이 아니라 텍스트로 명령어를 입력함으로써 조작하는 것을 말함

<br />

# 2. 쉘(Shell)

- 껍데기의 의미로 운영 체제 상에서 다양한 운영 체제 기능과 서비스를 구현하는 인터페이스를 제공하는 프로그램
- 커널(Kernel)와 직접적으로 연결되어 있으며, 커널과 사용자를 연결하여 사용자가 입력한 명령어를 해석하는 역할
- 사용자가 입력한 명령 라인을 읽어 해석하고 명령 라인이 실행되게 하는 명령 인터프리터(Command Interpreter)
<br /><br />
쉘은 키보드와 화면을 통해 사용자와 대화하는 인터페이스 기능을 제공하기도 하지만, 프로그램으로서의 강력한 프로그래밍 언어 기능도 가지고 있음<br />
- 사용자가 많은 명령을 사용하여 복잡한 작업을 수행하는 쉘 프로그램(쉘 스크립트) 파일을 작성해 사용자 자신만의 명령을 만들 수 있게 함
- 쉘 스크립트로 정의된 사용자지정 명령들은 /bin 디렉토리에 위치하고 있는 시스템 명령들과 동일한 상태를 가질 수 있음
>💡 bin은 binaries의 약자로 2진 파일들을 의미하며, /bin 디렉토리에는 가장 기본이 되는 명령어들이 모여있다.<br />
부팅에 필요한 명령어들도 위치하고 있으며, 시스템 사용자들이 사용할 수 있는 일반적인 명령어들도 위치하고 있다.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRsf1TQx0tHaax8JmsCTiCBMEsGNmegsvYv1g&usqp=CAU)<br />
<br/>
쉘의 종류에는 sh, csh(C프로그램 스타일의 Shell), ksh, bash 등이 있다.
<br /><br />

# 📚 Reference
리눅스마스터 1급, 지앤선
[터미널 사용방법](https://nam-ki-bok.github.io/backend/Backend_6/)<br />
[터미널 사용법 기초](https://yeonduing.tistory.com/19)<br />
[터미널과 CLI](https://dinfree.com/lecture/core/101_basic_3.html)

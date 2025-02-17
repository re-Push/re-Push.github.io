---
layout: single
title:  "리눅스 필기요약"
---
.
# 1. 왜 우리는 리눅스(Linux)를 배워야 하는가?
- 리눅스는 os의 한 종류이다 마치 우리가 평소에 사용하는 윈도우 같은 것이다. 우리는 평소에 윈도우 os안에서 게임을 하고 문서를 작성하는등 다양한 업무를 수행하지만 우리가 앞으로 사용할 프로그램들은 리눅스를 바탕으로 만들어졌기 떄문에, 리눅스os를 이용해야한다. 물론 윈도우에서도 프로그램이 작동할 수 있게 에뮬을 하 수 있지만 매 번 그렇게 사용하는것 보다 내가 os를 바꾸면 더 편하지 않은가!
- (요약) 서비스 하는 프로그램들이 대부분 리눅스환경에서 동작하기 때문이다.
# 2. 어떤 리눅스를 배워야 하는가?
- 앞으로 많이 이용할 가능성이 높은 것. 현재 많이 사용하는 것(커뮤니티가 잘 형성되어서 문제해결에 용이하다). 사용하기 편한 것.을 기준으로 선택하자.
- Debian계열과 그 중에서도 Ubuntu의 사용율이 증가하는 추세이다. Ubuntu의 어원을 따져보면 우리운영체제 이다. Ubuntu는 데스크탑, 그 중에서도 저사양 데스크탑을 겨냥해 만든 운영체제였다.
- (요약) Ubuntu, 많이 사용하니까.
# 3. 개발자가 알아야 할 리눅스의 필수 내용
- 리눅스는 보통 서비스관리를 위해 사용된다.
- 서비스 관리를 위해서 적용되는 내용을 탑투바텀으로 설명해보면, 서비스관리 - Tomcat/MySQL - JAVA JDK 설치 - Telnet/SSH/FTP - 설치파일 관리 - Bash Shell - 프로세스 관리 - 사용자 관리 - 파일관리 - 파일편집 - Linux 서버설치 - Linux/Unux 역사 정도가 되겠다.
- (요약) 서비스 관리를 위한 프로그램 Tomcat/MySQL을 다룰 줄 알면 된다.
# 4. 유닉스의 탄생과 운영체제의 의미
- 컴퓨터 성능이 좋아지면서 프로그램을 실행해도 성능이 남아도는 상황이 되었다. 그래서 기획된것이 Multics Project이다. Multics Project는 여러가지 프로그램을 멀티테스킹 할 수 있게 만드는 프로젝트였다. 비록 해당 프로젝트는 실패했지만 그곳에서 얻은 아이디어로 OS를 만들기 시작했다. 캔톰슨이라는 사람이 주크박스처럼 주크박스 안에 노래를 담아놓고 하나씩 꺼내서 사용하는 방식으로 os를 처음 만들었다. 그리고 운영체제에 종속된 프로그램이었기 때문에 하드웨어에 구애받지않고 운영체제만 맞다면 프로그램이 정상적으로 동작하게 되었다. 언어는 BCPL의 B를 따서 B언어를 기반으로 만들어졌다. 그러다가 컴퓨터의 성능이 더 좋아지면서 데이터의 크기가 커져서 각기 다른 데이터를 수용가능한 언어를 만들어야했다. 그래서 C언어가 만들어졌고 C언어를 기반으로 UNIX를 다시 만들게 되었다.
- (요약) 컴퓨터의 성능이 좋아지면서 탄생했다.
# 5. 오픈소스 유닉스의 탄생
- 유닉스가 유료화되면서 무료버전의 유닉스를 만들기위한 움직임이 시작되었다. 유료화가 된 이유는 AT&T가 독점하는걸 막기 위해 정부에서 AT&T를 7개의 회사로 분리시키면서 AT&T가 컴퓨터를 판매하지 못하게 되었다. 그러면서 수익을 내기 위해 각 컴퓨터들에 대해서 OS를 팔기 시작했다. 이에대해서 무료로 만들기 위해 GNU라는 조직을 만들고 FSF(Free Software Foundation)을 설립하기 시작한다. 말그대로 공짜유닉스를 처음부터 다시 만들어보자는 것이다. 하지만 Unix Kernel을 만들기가 어려웠는데 UC버클리에서 해결해낸다. 하지만 이에대해 AT&T가 소송을 했다 내부 자료를 이용해 재 작성한 코드이기 때문. 하지만 USL이 Novell로 팔리면서 소송이 취하된다. 이와중에도 여러 각지에서 무료유닉스를 만들고 있었는데 고가의 성능좋은 칩이아닌 저사양 인텔칩으로도 Unix를 사용할 수 있게 만들어서 뉴스그룹에 포스팅한다. 일종의 큰 커뮤니티였다. 이 글을 읽은 다른 사람들도 자신의 하드웨어에 맞게 이 사람이 만든 무료os를 바꾸어가며 수많은 소스코드를 만들어서 사용하고 다시 뉴스그룹에 올리고 수많은 Unix개보가 생기게 되었다. 그 개보가 이어지다가 Mac OS도 생기게 된 것이다.
- (요약) 독점을 막기위한 움직임이 유료화를 만들었고 이에대해 수많은 사람들의 노력으로 무료화된 수많은 OS들이 등장하게 되었다.
# 6. 오픈소스에도 라이센스가 있다.
- 오픈소스를 사용하기 이전에 해당 오픈소스는 어떤라이센스에 포함되어있는지를 확인하는 것이 중요하다.
- GPL(General Public License)라이센스, 모든 소스코드가 공개되어있지만 GPL이 적용된 SW를 만들었을시에 본인도 모든 소스를 공개해야한다.
- Apache 라이센스, 모든 소스코드를 공개할 필요는 없지만 저작권에대한 표시는 의무
- MIT 라이센스, 완전한 자유.
- (요약) 오픈소스 이용전에 라이센스를 먼저 잘 고르자
# 7. 리눅스 설치를 위한 virtual Box 설치하기
- 가상컴퓨터를 만들 수 있는 툴.
- 오라클홈페이지에 들어가서 다운로드에 들어가서 VM virtualbox를 다운로드한다. 가상머신 만들기에 들어가서 종류는 Linux 버전은 Ubuntu 64-bit으로 만들어준다. 만약 64-bit선택지가 없다면 64bit의 가상머신 자리가 없다는 건데 이는 크게 2가지 이유가 있을 수 있다. 하나는 이미 가상머신을 사용하고 있는 상태 또 하나는 BIOS 설정에서 가상화옵션이 꺼져있을 때 이다. 해결되었으면 리눅스 - 우분투 64비트 - 적당히 나눠줄 메모리크기 - 하드디스크 파일 종류는 다른 가상하드방식을 만들것인지 버츄얼박스에서만 쓰는 이미지를 만들것인지 설정 - 하드디스크의 크기를 사용한 만큼만 늘려가면서 사용할 것인가 동적할당을 설정해주고 - 적당한 하드디스크 크기를 결정한다. 끝.
- (요약) virtual box를 설치하고 가상머신을 만드는 과정
# 8. 우분투 18.04 Server 설치하기
- 우분투 홈페이지 - download - Ubuntu Server - Get Ubuntu Server - Option 2 Manual server installation - Download Ubuntu Server - 가상박스열고 설정 - 저장소 - 컨트롤러 비어있음 클릭 - 속성 - 디스크모양 클릭 - 가상 광디스크 파일 선택 - 방금 받은 파일 열기 - 확인 - 컴퓨터 부팅 - 설치언어 영어 - 레이아웃 한국어 - 인스톨러 첫번째 선택 - 이후 첫번쨰로 나오는 항목들 전부 선택해주고 - 이름 및 패스워드 설정 - 이후 특별한 설정 없이 설치 완료
- (요약) virtualbox에 우분투 설치하기
# 9.  Linux(Unix) 쉘과 프롬프트
- Bourn Shell을 이용해서 유닉스 시스템 사용 - 관리자 권한 얻기 - 명령프롬프트에서 - 아이디 패스워드를 입력하면 $ sign이 뜬다. 이러면 일반사용자 권한이고 이를 # pound sign으로 바꿔주어야 한다. sudo reboot 또는 sudo halt를 입력한는 방법이 있고 아예 root계정으로 전환하는 방법이 있다. sudo su - root 로 사용자를 전환하자 sudo는 super user do 의 약자이다.
- (요약) 일반사용자 권한에서 관리자 권한으로 들어가는 방법
# 10. Linux(Unix) 파일 시스템 구조
- 우리가 파일을 저장할 때 아무렇게나 저장할 수도 있겠지만 편의상 어디에 어떤 종류의 파일을 저장할지 정해놓는 것과 같은 원리이다. 이런저런 명칭에 따라 윈도우의 파일 시스템에 대응하는 것들이 있지만 지금은 그냥 간단하게 원리만 파악하고 직접 쓰면서 익히도록 하자
- (요약) 파일을 정리하는 기준
# 11. Linux(Unix) 파일 경로와 순회
- 파일 탐색을 위한 명령어들 pwd(print working dirictoty) 현재 디렉토리 경로를 출력 ls(list) 디렉토리 목록 나열 cd(change directoty) 디렉토리를 변경 ../ 부모에게 가겠다 ~(tilde 틸드기호) 내 홈디렉토리를 나타내는 특수한 기호이다 ls -l(list라는 뜻) 파일에 대한 정보를 자세하게 보여준다. 사용자의 권한, 소유자 그룹, 크기, 날짜 등을 자세하게 보여준다. man ls 라고 입력하면 메뉴얼을 보여준다 하지만 내용이 너무 방대해서 내가 필요한 부분만 인터넷에 검색을 해서 찾아보는게 낫다.
- (요약) 간단하게 파일간의 이동을 하는 방법들에 대한 내용이다.
# 12. Linux(Unix) 파일 관리 명령어
- mkdir 디렉토리 생성 make directory
- rmdir 디렉토리 삭제
- touch 빈 파일 생성
- mv 파일 이동 / 변경 move
- rm 파일 삭제 remove      rm -r 하면 디렉토리 안쪽에있는 모든 파일까지 제거      rm -ri 상호작용하면서 지우겠다는 이야기
- cp 파일 복사 copy
- (요약) GUI에서는 간단하게 사용했던 파일 추가제거 기능들이 CLI에서는 하나하나 지정해주는 내용을 숙지해야한다.
# 13. Linux(Unix)파일 편집 및 관리
- 파일 편집기에는 VI GNU nano Emacs ed/ex 가 있는데 그중에서 오늘은 VI편집기에 대해서 배운다 VI 편집기에는 쉘 명령모드 편집 다시 명령모드 해서 빠져나오는 순서로 편집이 이루어진다 쉘에서 vi 와 이름을 통해 들어가고 들어가면 명령모드로 들어가진다 이 상태에서 i는 현재위치에서 편집하기 o는 현재위치의 다음 줄에서 편집하기가 가능하다. 그리고 명령모드에서 yy yw yl은 각각 문장 단어 글자를 복사할 수 있고 p를 통해 붙여넣기가 가능하다 esc를 누르면 다시 명령모드로 들어가진다 나가기 전에 명령모드에서 :w 를 눌러서 저장을 하고 :q를 눌러서 나가면 된다 연결해서 :wq 를 입력하면 저장하고 나가기가 가능하다 추가적으로 hjkl을 이용해 명령모드에서 위 아래 양옆으로 이동이 가능하다
- (요약) 파일에 들어가서 편집을 하고 저장하고 나오는 내용이다.
# 14. Linux(Unix) 나노(nano)를 이용한 파일편집
- editor 또는 nano 에서 편집시작이 가능하다. nano로 편집하러 들어가면 아래에 필요한 기능에대한 키가 잘 정리되어 있기 때문에 잘 보고 이용하면 된다.
- (요약) nano를 이용한 파일편집.
- (추가내용) capital을 치고 tap키를 눌러주면 그 단어를 포함한 유일한 디렉토리 하나를 불러온다 만약 겹치는 이름의 디렉토리가 있다면 tap키를 2번 눌러주면 선택지가 나오는데 원하는 디렉토리의 이름을 어느정도 더 채워주고 다시 tap키를 누르면 완성된 해당 디렉토리 이름이 나오게된다.
# 15.  Linux(Unix) 파일 찾기와 파일 정보 확인하기(find, file, cmp, cat, head, tail, which)
- 



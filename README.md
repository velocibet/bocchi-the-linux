# Bocchi the Linux (v0.1)

<img width="1920" height="1080" alt="Screenshot_20260321_112350" src="https://github.com/user-attachments/assets/b4a7125b-4a81-4a93-8b98-0d8315f87bbb" />

---

> "아치 리눅스도... 무섭지 않아!"  

KDE Plasma 기반의 '봇치 더 록!' 테마 커스텀 Arch Linux 프로젝트입니다. (현재 야마다 료 테마만 사용 가능)

## 주요 특징
- **Desktop:** KDE Plasma 6
- **Input:** IBus-Hangul 한글 입력기 기본 설정
- **Tools:** Fastfetch, Firefox, Dolphin, Konsole, Bocchifetch 탑재
- **Wallpaper:** 야마다 료 배경화면 적용

---

## Bocchifetch
<img width="1034" height="433" alt="Screenshot_20260325_233358" src="https://github.com/user-attachments/assets/ce762da6-ff03-455a-9286-57e512d9acfa" />

터미널에 ``bocchifetch``를 이용해 시스템 사양을 출력할 수 있습니다. 귀여운 료와 함께 시스템 사양을 구경해보세요!

---

> [!CAUTION]
> ## 주의
> 본 리눅스 배포판은 아직 미완성으로 완전하지 않습니다. 파티셔닝 기능이 제공되지 않습니다. 
> 실제 사용 중인 컴퓨터에 설치하는 것을 권장하지 않으며, 사용하지 않는 USB에 재미로만 설치하는 것을 권장합니다.
> 이 배포판을 이용하는데 발생한 문제의 책임에 있어서는 전적으로 사용자에게 책임이 있습니다.

---

## 다운로드
3GB 이상의 USB가 필요합니다.

1. [Releases (현재 최신 버전 v0.1)](https://github.com/velocibet/bocchi-the-linux/releases/tag/v0.1) 페이지에서 ISO 파일을 다운로드 합니다.
2. 설치 USB 만들기
- 윈도우의 경우 [Refus](https://rufus.ie/ko/#download)를 이용해 USB에 다운로드한 ISO 파일을 굽습니다.
- 리눅스의 경우 **gnome-multi-writer**을 이용해 굽습니다. 설치 방법은 리눅스 배포판 별로 다음과 같습니다.
- Arch Linux:
``
sudo pacman -S gnome-multi-writer
``

- Ubuntu (Debian 계열):
``
sudo apt update && sudo apt install gnome-multi-writer
``

- Fedora (RedHat 계열):
``
sudo dnf install gnome-multi-writer
``

3. 펌웨어에서 설치 USB로 부팅합니다.
4. 먼저 설치하기에 앞서 인터넷에 연결합니다. (유선 랜인 경우, 이 항목을 건너 뛰고 5번으로 넘어가도 괜찮습니다.)
- 가장 쉬운 방법은 ``archinstall`` 명령어를 친 후에 인터넷 연결을 하고 설치를 취소하는 방법입니다.
- 만약 수동으로 연결하고자 할 경우, iwctl을 이용해 연결합니다. 자세한 방법은 이 [블로그](https://digiconfactory.tistory.com/entry/%EB%A6%AC%EB%88%85%EC%8A%A4%EC%97%90%EC%84%9C-iwd%EB%A1%9C-%EB%AC%B4%EC%84%A0-WIFI-%EC%97%B0%EA%B2%B0) 내용을 참고하십시오.
- 무선 랜에 연결되었는지 확인하는 방법은 ``ip link`` 명령어 입력 후 아래에 wlan0 또는 wlp2s0(무선 랜카드를 의미합니다.)가 'UP'이라고 출력되는지 확인하십시오. 만약 'DOWN'이라고 뜬다면 무선 와이파이에 연결되지 않은 것입니다.
5. 이후 ``sudo bocchi-installer`` 명령어를 입력한 후 명령에 따라 설치를 진행합니다.
- 만약 해당 명령어를 입력하였으나 명령어가 존재하지 않는다고 뜬다면 해당 인스톨러에 권한이 없는 것입니다. (이 경우엔 ``sudo chmod 755 /usr/bin/bocchi-installer``을 입력하여 인스톨러에 관리자가 실행할수 있는 권한을 부여하십시오.)
6. 설치 중 ``Enter password for archuser`` 라고 출력이 뜬다면 비밀번호를 입력하면 됩니다. 이 비밀번호는 root 비밀번호로도 설정됩니다.
7. 설치가 완료되었다면, usb 제거 후 재부팅합니다.
8. 기본 디스플레이는 KDE 입니다. 바탕화면 우클릭 후 설정으로 들어가 배경화면을 기본 내장된 야마다 료의 사진으로 변경할수 있으며, 몇가지 KDE 테마도 설치되어 있습니다.

## 일러두기
- 현재는 KDE Plasma, Ibus 한글 입력기, Firefox와 같은 필수적인 기능만 들어가 있습니다.
- 별도의 프로그램은 KDE Discover 또는 pacman 명령어로 설치가 가능합니다.
- 후에 커미션을 통해 테마를 꾸밀 예정입니다.
- 현재는 개발자의 숙련도 부족으로 KDE로 제작되어 있으나 후에 Hyprland와 같은 별도의 데스크탑 환경으로 변경될 수 있습니다.
- 피드백 및 이슈, 풀 리퀘스트는 언제든지 환영합니다.
- Bocchi-install, Bocchifetch는 Rust로 작성되었습니다.

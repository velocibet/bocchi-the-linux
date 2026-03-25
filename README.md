# Bocchi the Linux (v0.1)

<img width="1920" height="1080" alt="Screenshot_20260321_112350" src="https://github.com/user-attachments/assets/b4a7125b-4a81-4a93-8b98-0d8315f87bbb" />

---

> "아치 리눅스도... 무섭지 않아!"  

KDE Plasma 기반의 '봇치 더 록!' 테마 커스텀 Arch Linux 프로젝트입니다. (현재 야마다 료 테마만 사용 가능)

## 주요 특징
- **Desktop:** KDE Plasma 6
- **Input:** IBus-Hangul 한글 입력기 기본 설정
- **Tools:** Fastfetch, Firefox, Dolphin, Konsole 탑재
- **Wallpaper:** 야마다 료 배경화면 적용

## 다운로드
4GB 이상의 USB가 필요합니다.

1. [Releases](링크) 페이지에서 ISO 파일을 다운로드 합니다.
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

- Fedora OS (RedHat 계열):
``
sudo dnf install gnome-multi-writer
``
3. 설치 USB로 부팅 후 Arch linux를 설치합니다.

## 일러두기
- 현재는 KDE Plasma, Ibus 한글 입력기, Firefox와 같은 필수적인 기능만 들어가 있습니다.
- 별도의 프로그램은 KDE Discover 또는 pacman 명령어로 설치가 가능합니다.
- 후에 커미션을 통해 테마를 꾸밀 예정입니다.
- 현재는 개발자의 숙련도 부족으로 KDE로 제작되어 있으나 후에 Hyprland와 같은 별도의 데스크탑 환경으로 변경될 수 있습니다.
- 피드백 및 이슈, 풀 리퀘스트는 언제든지 환영합니다.

# TabSpacePlay

Armbian 기반 Apple AirPlay를 지원하는 TabSpace의 OS입니다.


# Command

apt update && apt upgrade -y

apt install shairport-sync

systemctl enable shairport-sync

armbian-config
- enable analog-codec

alsamixer
- Line Out and DAC Volume MAX

renice -n -19 -u shairport-sync

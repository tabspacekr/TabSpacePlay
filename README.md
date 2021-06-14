# TabSpacePlay

1) Armbian 기반 Apple AirPlay를 지원하는 TabSpace의 OS입니다.

2) MultiRoom 동시재생 솔루션을 Balena Sound 솔루션을 활용하여 제공합니다.

# Installation Command : Method A

apt update && apt upgrade -y

apt install shairport-sync

systemctl enable shairport-sync

armbian-config
- enable analog-codec

alsamixer
- Line Out and DAC Volume MAX

renice -n -19 -u shairport-sync

# Installation Command : Method B

wget https://raw.githubusercontent.com/tabspacekr/TabSpacePlay/main/ogpi_airplay_install.sh

chmod a+x ogpi_airplay_install.sh

./ogpi_airplay_install.sh

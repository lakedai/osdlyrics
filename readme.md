### change metadata to get real title and artist
- if no tag, find title / artist from meta title
- support meta title formats: %n.%p-%t, %n.%t--%p, %n.%t, %p-%t, %t--%p, %t
- default download changes to download best match first

### changed src files:
- 修改：     README.md
- 增加：     readme.md
- 修改：     po/zh_CN.po
- 修改：     src/ol_lyric_candidate_selector.c
- 修改：     src/ol_main.c
- 修改：     src/ol_metadata.c
- 修改：     src/ol_metadata.h
- 修改：     src/ol_player.c

### install instruction:
	sudo apt install osdlyrics
	./autogen.sh
	./configure --prefix=/usr PYTHON=/usr/bin/python3
	make
	sudo cp src/osdlyrics /usr/bin

### build required:(ubuntu20.04)
- autoconf automake libtool
- libglib2.0-dev
- libgtk2.0-dev
- libdbus-glib-1-dev
- libnotify-dev
- intltool
- libappindicator-dev

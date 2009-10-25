This document explains how to properly build an Android package of Orbot from
source.

Please install the following prerequisites:
	Android OS SDK
	droid-wrapper: http://github.com/tmurakam/droid-wrapper
	libevent source
	Tor source (most recent git master branch)

Install and prepare the Android OS SDK ( http://source.android.com/download )
on Debian Lenny:

	sudo apt-get install git-core gnupg sun-java5-jdk flex bison gperf \
		libsdl-dev libesd0-dev libwxgtk2.6-dev build-essential zip \
		curl libncurses5-dev zlib1g-dev

	curl http://android.git.kernel.org/repo >~/bin/repo
	chmod a+x ~/bin/repo

	mkdir ~/mydroid
	cd ~/mydroid

	repo init -u git://android.git.kernel.org/platform/manifest.git
	repo sync

	# Paste in key from http://source.android.com/download next...
	gpg --import

	export ANDROID_JAVA_HOME=$JAVA_HOME
	cd ~/mydroid
	make

XXX TODO: Explain build process for making a static Tor with our libevent, etc.
XXX TODO: Explain build process for making a .apk file for install.

# Avro phonetic for Linux in IBus
Avro phonetic implementation for Linux in IBus.

## Installation

On Ubuntu, and on Debian's *testing* and *unstable* releases, Avro phonetic
is distributed through the `ibus-avro` package. To install it, simply do:

	sudo apt install ibus-avro

On other Linux distros you can install the dependencies and build/install
using the source code in this repository.

1. Open terminal/package manager and install following packages:

		git
		libibus-1.0-dev
		automake
		autoconf
		make
		gjs
		ibus

		__For Fedora 35__
		sudo dnf install git automake autoconf make gjs ibus ibus-devel

		__AlmaLinux 8.5__
		sudo dnf install git automake autoconf make gjs ibus
		sudo dnf install epel-release
		sudo dnf install yum-utils
		sudo dnf config-manager --set-enabled powertools
		sudo dnf update
		sudo dnf install ibus-devel


    __For e.g. Debian 10 "buster"__

    As root, do:

		apt install git libibus-1.0-dev automake autoconf make gjs ibus



    __For other linux distributions__

    You'll need all related build tools like `automake`, `autoconf` etc...
    and to run it you need `ibus` and `gjs`. Use the list of packages above
    as guidance, but please note that some packages may have other names.

2. Now give the following commands step-by-step:

		git clone git://github.com/sarim/ibus-avro.git
		cd ibus-avro
		aclocal && autoconf && automake --add-missing
		./configure --prefix=/usr
		sudo make install

		__Note for Fedora 35__
		Modify "configure.ac" file if you encounter errors and run from "aclocal" command
		AM_INIT_AUTOMAKE(ibus-avro, 1.1)
		to
		AM_INIT_AUTOMAKE



## Usage
 1. Run __IBus__ (`Applications -> System Tools -> IBus`) from _Dash_
 2. Open __IBus__ `Preferences` from the top panel icon  
 3. Go to `Input method`
 4. `Select an input method -> Bengali -> Avro`
 5. Now Click `Add` button to add __Avro__ to the list
 6. Now restart __IBus__ from the top panel icon (`Right Click -> Restart`)
 7. Now Press `Ctrl+Space` to toggle between _English_ and _Avro_ (Bengali)
 8. Enjoy __Avro Phonetic!__

## Usage Fedora 35
  1. Log out and log back in. Better if you restart your machine.
	2. Go to `Settings -> Keyboard -> Input Sources`
	3. Click `+` to add new language.
	4. Click the ':' and start typing `avro`
	5. From Bangla(Bangladesh) select `Avro-Phonetic`
  6. Now Press `Ctrl+Space` to toggle between _English_ and _Avro_ (Bengali)
  7. Enjoy __Avro Phonetic!__

## Usage AlmaLinux 8.5
  1. Log out and log back in. Better if you restart your machine.
	2. Go to `Settings -> Region and Language -> Input Sources`
	3. Click `+` to add new language.
	4. Click the ':' and start typing `avro`
	5. From Bangla(Bangladesh) select `Avro-Phonetic`
  6. Now Press `Ctrl+Space` to toggle between _English_ and _Avro_ (Bengali)
  7. Enjoy __Avro Phonetic!__




## Contributors

__IBus Engine__ by __Sarim Khan__ <sarim2005@gmail.com>

[__Avro JavaScript Phonetic Library__](https://github.com/torifat/jsAvroPhonetic) by [__Rifat Nabi__](https://github.com/torifat)

__Avro Phonetic Dictionary Search Library__ by [__Mehdi Hasan Khan__](https://github.com/omicronlab)

_Licensed under Mozilla Public License 2.0 ("MPL"), an open source/free software license._

__Fedora 35 instructions__ by __M. Shahnoor Rahman__ <shahnoor3pl@gmail.com>

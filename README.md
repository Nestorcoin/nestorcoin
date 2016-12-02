Nestorkoin - the coin of freedom!

Nestorcoin integration/staging tree

http://nestorcoin.com

Blockexplorer

http://nestorcoin.com/block

DOWNLOAD

windows-qt

https://github.com/Nestorcoin/windows-qt

nestorcoin-qt-linux

https://github.com/Nestorcoin/nestorcoin-qt-linux.tar

nestorcoin-daemon-linux

https://github.com/Nestorcoin/nestorcoin-daemon-linux

What is Nestorcoin?

Nestorcoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.

License

Nestorcoin is released under the terms of the MIT license. See COPYING for more information or see

Development process

Developers work in their own trees, then submit pull requests when they think their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Nestorcoin development team members simply pulls it.

If it is a more complicated or potentially controversial change, then the patch submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing. Developers should expect to rework and resubmit patches if the code doesn't match the project's coding conventions (see doc/coding.txt) or are controversial.

The master branch is regularly built and tested, but is not guaranteed to be completely stable. Tags are created regularly to indicate new official, stable release versions of Nestorcoin.

Order type	paid

Algorithm	Scrypt

Type	PoW

Coin name	Nestorcoin

Coin abbreviation	NST

Address letter	N

RPC port	9248

P2P port	9247

Block reward	50 coins

Block halving	210000 blocks

Total coin supply	42000000 coins

Coinbase maturity	20 blocks

Target spacing	5 minutes

Target timespan	10 minutes

Transaction confirmations	6 blocks

Nestorkoin gives freedom

Install daemon (ubuntu 12, 14)

root@

Set up a swapfile if your system has less than 1.5GB of memory:

fallocate -l 2G /swapfile

chown root:root /swapfile

chmod 0600 /swapfile

mkswap /swapfile

swapon /swapfile

If fallocate doesn’t work, you can use dd if=/dev/zero of=/swapfile bs=1024 count=1024288 instead.

Initialize swapfile automatically on boot

Pull the source code from github, or upload it yourself:

apt-get install nano

nano /etc/fstab

Add this at the bottom: /swapfile none swap sw 0 0

Install all required dependencies:

apt-get update && apt-get upgrade

apt-get install ntp unzip git build-essential libssl-dev libdb-dev

apt-get install libdb++-dev libboost-all-dev libqrencode-dev

apt-get install aptitude

aptitude install miniupnpc libminiupnpc-dev

Pull the source code from github, or upload it yourself

git clone https://github.com/Nestorcoin/nestorcoin.git nestorcoin

cd nestorcoin/src/leveldb

chmod 0777 ./build_detect_platform

make libleveldb.a libmemenv.a

cd ..

make -f makefile.unix USE_UPNP=1 USE_QRCODE=1 USE_UPNP=1

strip nestorcoind

cp nestorcoind /usr/bin

cd ~

nestorcoind

oops! )))

mkdir .nestorcoin

nano .nestorcoin/nestorcoin.conf

Writes the data in the editor

rpcuser=your nickname

rpcpassword=your strong password

rpcport=9248

port=9247

addnode=93.170.169.165

listen=1

daemon=1

server=1

exit shortcuts

ctrl+х

y

enter

nestorcoind

terminal response "nestorcoin server starting"

Yes!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

GOOD MINING!

Nestorkoin - the coin of freedom!

Contacts

mailnestorcoin@gmail.com

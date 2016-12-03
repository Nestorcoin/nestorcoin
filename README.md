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

Nestorcoin is a lite version of Litecoin using scrypt as a proof-of-work algorithm.

License

Nestorcoin is released under the terms of the MIT license. See COPYING for more information or see

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

Premine amount	21000000 coins

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

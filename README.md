## Timmycoin (TMY)

<p align="center">
  <img src="https://github.com/tmycoin/timmy/blob/master/logo.png" width="250" />
</p>

> Based on CryptoNote Technology Timmycoin (TMY) COIN

**Website:** [www.timmycoin.net](https://www.timmycoin.net)

**Web Wallet:** [wallet.timmycoin.net](https://wallet.timmycoin.net)

**Explorer:** [explorer.timmycoin.net](https://explorer.timmycoin.net/)

**Roadmap:** [Roadmap](https://www.timmycoin.net/roadmap)

**BitcoinTalk:** [BitcoinTalk](https://bitcointalk.org/index.php?topic=5100223)

### Socials

**Telegram:** [tmycoin](https://t.me/timycoin)

**Twitter:** [tmycoin](https://www.twitter.com/tmycoin)

**Instagram:** [tmycoin](https://www.instagram.com/tmycoin)

_____

#### Build instructions


##### Dependency Ubuntu & Debian

Build requirements:

    apt-get install cmake build-essential libtool autotools-dev autoconf pkg-config libssl-dev libboost-all-dev

##### Dependency Mac OS X

Build requirements:

    brew install autoconf automake libtool boost miniupnpc openssl pkg-config protobuf qt5

##### Building Timmy

Clone the github tree to get the source code and go into the directory.

    git clone https://github.com/tmycoin/timmy.git
    cd timmy

Build Timmy

    make -j4

**Parallel build:** run `make -j<number of threads>` instead of make'.

**Debug build:** run `make build-debug`.

**Test suite:** run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.


## On Windows:

### Dependencies

* MSVC 2013 or later
* CMake 2.8.6 or later, 
* Download [boost_1_65_1-msvc-14.1-64](https://netix.dl.sourceforge.net/project/boost/boost-binaries/1.65.1/boost_1_65_1-msvc-14.1-64.exe) and install to `C:\local\boost_1_65_1` directory.



##### To build, change to a directory where this file is located, and run this commands: (VisualStudio 2015)

and add variables 

    BOOST_LIBRARYDIR=C:\local\boost_1_65_1\lib64-msvc-14.1
    BOOST_ROOT=C:\local\boost_1_65_1

clone and build

    git clone https://github.com/tmycoin/timmy.git
    cd timmy
    cd build
    cmake .. -G "Visual Studio 15 2017 Win64" ..

then open **Timmycoin.sln** File on Visual Studio

In VS' Solution Explorer select upnpc-static' Properies -> C/C++ -> Code Generation -> Runtime Library - > change it to Multi-threaded (/MT)


#### Nodes

```C
const char* const SEED_NODES[] = {
  "timmy-1.timmycoin.net:1302",
  "timmy-2.timmycoin.net:1302",
};
```

#### Offical TMY WALLET:

    9Jxgz7zacYtAcx7kXFLYeSgG3VrjCSVKBP2Nzc88YY7rWxtTz4zksyNYGMWLZ4tLV7hVy9hRDf69XZ5qvnSCUUsZPqb7DNQ

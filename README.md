## Timmycoin (TMY)

> Based on CryptoNote Technology Timmycoin (TMY) COIN

**Website:** [www.timmycoin.net](https://www.timmycoin.net)

**Web Wallet:** [wallet.timmycoin.net](https://wallet.timmycoin.net)

**Explorer:** [explorer.timmycoin.net](https://explorer.timmycoin.net/)

**Roadmap:** [Roadmap](https://www.timmycoin.net/roadmap)

**BitcoinTalk:** [BitcoinTalk](https://---)

##### Socials

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


### On Windows:

##### Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55 or later. You may download them from:

http://www.microsoft.com/

http://www.cmake.org/

http://www.boost.org/

##### To build, change to a directory where this file is located, and run this commands: (VisualStudio 2015)

    mkdir build && cd build && cmake .. -G "Visual Studio 14 Win64" ..

then open **Timmycoin.sln** File on Visual Studio

In VS' Solution Explorer select upnpc-static' Properies -> C/C++ -> Code Generation -> Runtime Library - > change it to Multi-threaded (/MT)


#### Nodes

```C
const char* const SEED_NODES[] = {
  "timmy-1.timmycoin.net:1302",
  "timmy-2.timmycoin.net:1302",
};
```

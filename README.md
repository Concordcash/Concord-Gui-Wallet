# Concord Wallet (GUI)
Latest Release: v0.0.4
Maintained by Concord.

## Warning: This is Highly Experimental for testing purposes, Use at own Risk!

## Information
### Concord

The Future Of Blockchain 

Concord is a decentralized cryptocurrency based on the cryptonote protocol. Concord is the complete solution for your blockchain Banking, Payment, and Messaging needs. It also provides instant privacy protected peer-to-peer transactions as well as untraceable/self-destructive encrypted messaging, with extremely low processing fees in a decentralized network.

- Coin Name: Concord
- Genesis Date: 15-July-2021
- Ticker: CCR
- Address Prefix: CCR
- POW Algo: Cryptonight Arto
- Block Time: 180 seconds
- Max Supply: 100 million
- Block Reward: 5-50
- Ports:
- P2P: 33526
- RPC: 33590


## Resources
- Web: [Concord.cash](https://Concord.cash/)
- GitHub: [https://github.com/Concordcash/Concord-Cash](https://github.com/Concordcash/Concord-Cash)
- Discord: 
- BitcoinTalk: https://bitcointalk.org/index.php?topic=5350834
- Telegram: 
- Twitter: 
- Facebook: 
- Medium: 
- Cryptunit: 

### [Block Explorer] 
- https://explorer.Concord.cash/

### [Remote Node]
- node.Concord.cash

### [Pools] 
- https://pool.Concord.cash


## Compiling Concord from source

### Linux / Ubuntu

##### Prerequisites

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, Boost 1.55 or later, and Qt 5.9 or later.
You may download them from:

- http://gcc.gnu.org/
- http://www.cmake.org/
- http://www.boost.org/
- https://www.qt.io

Alternatively, it may be possible to install them using a package manager.

#### Building

To acquire the source via git and build the release version, run the following commands:

- `cd ~`
- `git clone https://github.com/Concordcash/Concord-Gui-Wallet ccrgui`
- `cd ccrgui`
- `make build-release`
- `mkdir bin && mv build/release/Concord-GUI bin/`
- `make clean`

If the build is successful the binaries will be in the bin folder.

### Windows 10

##### Prerequisites

- Install [Visual Studio 2017 Community Edition](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15&page=inlineinstall)
- When installing Visual Studio, you need to install **Desktop development with C++** and the **VC++ v140 toolchain** components. The option to install the v140 toolchain can be found by expanding the "Desktop development with C++" node on the right. You will need this for the project to build correctly.
- Install [CMake](https://cmake.org/download/)
- Install [Boost 1.67.0](https://boost.teeks99.com/bin/1.67.0/), ensuring you download the installer for MSVC 14.1.
- Install [Qt 5.11.0](https://www.qt.io/download)

##### Building

- From the start menu, open 'x64 Native Tools Command Prompt for vs2017' or run "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\Tools\VsMSBuildCmd.bat" from any command prompt.
- Edit the CMakeLists.txt file and set the path to QT cmake folder. For example: set(CMAKE_PREFIX_PATH "C:\\Qt\\5.11.0\\msvc2017_64\\lib\\cmake\\").
- `git clone https://github.com/Concordcash/Concord-Gui-Wallet ccrgui`
- `cd ccrgui`
- `mkdir build`
- `cd build`
- `cmake -G "Visual Studio 15 2017 Win64" -DBOOST_LIBRARYDIR:PATH=c:/local/boost_1_67_0 ..` (Or your boost installed dir.)
- `msbuild concordwallet.sln /p:Configuration=Release`

If the build is successful the binaries will be in the Release folder.

#### Special Thanks
Special thanks goes out to the developers from Cryptonote, Bytecoin, Monero, Forknote, TurtleCoin, Masari, The Circle Team


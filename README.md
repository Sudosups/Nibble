# Nibble Core (CLI)
Latest Release: v4.0.0
Maintained by The Nibble Developers

![Ubuntu 16.04](https://github.com/Sudosups/Nibble/workflows/Ubuntu%2016.04/badge.svg?branch=master)

## Information
Nibble is based on the Conceal Network project. Nibble is a decentralized reward platform with encrypted messages and own privacy protected cryptocurrency.

All your XCR transactions and messages are anonymous. The Nibble Network provides an instant secure, untraceable and unlinkable way of encrypted communication - crypto messages.

Nibble is open-source, always has been and always will be. 
This latest edition of Nibble, has been created from a merger of projects - Nibble Classic & Crumbs
Giving our users the best from both worlds, a simple to use platform, messaging ability, deposits & rewards.

## Resources
- Web: https://nibble-nibble.com
- GitHub: https://github.com/Nibble-Network/Nibble
- Discord: 
- Twitter: 
- Bitcoin Talk: 
- Paperwallet: 

## Compiling Nibble from source

### Linux / Ubuntu

##### Prerequisites

- You will need the following dependencies to build the Nibble CLI: boost, cmake, git, gcc, g++, python, and make.
- On Ubuntu: `sudo apt-get install -y build-essential python-dev gcc g++ git cmake libboost-all-dev`

#### Building

- `git clone https://github.com/Nibble-Network/Nibble`
- `cd nibble-core`
- `mkdir build && cd $_`
- `cmake ..`
- `make`

If the build is successful the binaries will be in the src folder.

### Windows 10

##### Prerequisites

- Install [Visual Studio 2019 Community Edition](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=Community&rel=16)
- Install [CMake](https://cmake.org/download/)
- When installing Visual Studio, you need to install **Desktop development with C++** and the **MSVC v142 - VS 2019 C++ x64/x86 build tools** components. The option to install the v142 build tools can be found by expanding the "Desktop development with C++" node on the right. You will need this for the project to build correctly.
- Use the premade binaries for [MSVC 14.2]
- Install [Boost 1.70.0](https://sourceforge.net/projects/boost/files/boost-binaries/1.70.0/boost_1_70_0-msvc-14.1-64.exe/download), ensuring you download the installer for MSVC 14.2.

##### Building

- From the start menu, open 'x64 Native Tools Command Prompt for vs2019' or run "C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\Common7\Tools\VsMSBuildCmd.bat" from any command prompt.

- `git clone https://github.com/Nibble-Network/Nibble`
- `cd nibble-core`
- `mkdir build`
- `cd build`
- `cmake -G "Visual Studio 16 2017" -A x64 -DBOOST_LIBRARYDIR="c:\local\boost_1_70_0\lib64-msvc-14.2 ..` (Or your boost installed dir.)
- `msbuild nibbleX.sln /p:Configuration=Release /m`

If the build is successful the binaries will be in the src/Release folder.

### macOS

#### Prerequisites

In order to install prerequisites, [XCode](https://developer.apple.com/xcode/) and [Homebrew](https://brew.sh/) needs to be installed.
Once both are ready, open terminal app, run following command:

```bash
$ xcode-select --install
```

and install all tools. On newer macOS versions (v10.14 and higher) this step is done through Software Update app.

After that, proceed with installing dependencies:

```bash
$ brew install git python cmake gcc boost
```

When all dependencies are installed, build nibble Core binaries:

```bash
$ `git clone https://github.com/Nibble-Network/Nibble`
$ `cd nibble-core`
$ mkdir build && cd $_
$ cmake ..
$ make
```

If the build is successful the binaries will be located in `src` directory.

#### Special Thanks
Special thanks goes out to the developers from Cryptonote, Bytecoin, Monero, Forknote, TurtleCoin, Karbo, Masari & Conceal Network.

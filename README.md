Flyt v1.0.2 is based on the [CryptoNote](https://cryptonote.org) cryptocurrency protocol.
Current blockchain is mining difficulty around 10 and current reward is 9.5 blocks.
Each block is discounted. 

* CryptoNote reference implementation: [CryptoNoteCoin](https://cryptonote-coin.org)
* Discussion board and support: [CryptoNote Forum](https://forum.cryptonote.org)

### Preparation

1. Create an account on [GitHub.com](github.com)
2. Fork [VolleyCoin repository](https://github.com/shopglobal/volleycoin)
3. Buy one or two Ubuntu-based dedicated servers (at least 2Gb of RAM) for seed nodes.

## Building Flyt 

### On *nix

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.55.

You may download them from:

* http://gcc.gnu.org/
* http://www.cmake.org/
* http://www.boost.org/
* Alternatively, it may be possible to install them using a package manager.

To build, change to a directory where this file is located, and run `make`. The resulting executables can be found in `build/release/src`. 

cd build/release/src && ./flytd
Happy mining!


**Advanced options:**

* Parallel build: run `make -j<number of threads>` instead of `make`.
* Debug build: run `make build-debug`.
* Test suite: run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.
* Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++` before running `make`.

### On Windows
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55. You may download them from:

* http://www.microsoft.com/
* http://www.cmake.org/
* http://www.boost.org/

To build, change to a directory where this file is located, and run these commands: 

Windows Executable
```
mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..
```

And then do Build.
Good luck!

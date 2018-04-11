# WebAssembly
Repository for learning WebAssembly

## Instalation PreRec
See [Developers Guide](http://webassembly.org/getting-started/developers-guide/)
### Linux Installs
***This was written for an install of wheezy on chroot***

#### GIT
See [GIT Install](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

```sudo apt install git-all```
#### CMAKE
See [CMAKE Install](http://cgold.readthedocs.io/en/latest/first-step/installation.html)

```sudo apt-get -y install cmake```
#### GCC
See [GCC Install](https://askubuntu.com/questions/154402/install-gcc-on-ubuntu-12-04-lts)

```sudo apt-get install gcc```

#### Python 2.7
See [Python 2.7 Install](https://askubuntu.com/questions/101591/how-do-i-install-the-latest-python-2-7-x-or-3-x-on-ubuntu)

Dependancys:

```sudo apt-get install build-essential checkinstall```

```sudo apt-get install libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev```

```version=2.7.13```

```cd ~/Downloads/```

```wget https://www.python.org/ftp/python/$version/Python-$version.tgz```

```tar -xvf Python-$version.tgz```

```cd Python-$version```

```./configure```

```make```

```sudo checkinstall```

output:
```
**********************************************************************

 Done. The new package has been installed and saved to

 /home/ico/Downloads/Python-2.7.13/python_2.7.13-1_amd64.deb

 You can remove it from your system anytime using: 

      dpkg -r python

**********************************************************************
```

#### Toolkit


```git clone https://github.com/juj/emsdk.git```

```cd emsdk```

```./emsdk install latest```

```./emsdk activate latest```

Output:
```
The Emscripten configuration file /home/ico/.emscripten has been rewritten with the following contents:

import os
LLVM_ROOT='/home/ico/emsdk/clang/e1.37.36_64bit'
EMSCRIPTEN_NATIVE_OPTIMIZER='/home/ico/emsdk/clang/e1.37.36_64bit/optimizer'
BINARYEN_ROOT='/home/ico/emsdk/clang/e1.37.36_64bit/binaryen'
NODE_JS='/home/ico/emsdk/node/8.9.1_64bit/bin/node'
EMSCRIPTEN_ROOT='/home/ico/emsdk/emscripten/1.37.36'
SPIDERMONKEY_ENGINE = ''
V8_ENGINE = ''
TEMP_DIR = '/tmp'
COMPILER_ENGINE = NODE_JS
JS_ENGINES = [NODE_JS]

To conveniently access the selected set of tools from the command line, consider adding the following directories to PATH, or call 'source ./emsdk_env.sh' to do this for you.

   /home/ico/emsdk:/home/ico/emsdk/clang/e1.37.36_64bit:/home/ico/emsdk/node/8.9.1_64bit/bin:/home/ico/emsdk/emscripten/1.37.36
Set the following tools as active:
   clang-e1.37.36-64bit
   node-8.9.1-64bit
   emscripten-1.37.36
```

```source ./emsdk_env.sh --build=Release```

Output:
```
(wheezy)ico@localhost:~/emsdk$ source ./emsdk_env.sh --build=Release
Adding directories to PATH:
PATH += /home/ico/emsdk
PATH += /home/ico/emsdk/clang/e1.37.36_64bit
PATH += /home/ico/emsdk/node/8.9.1_64bit/bin
PATH += /home/ico/emsdk/emscripten/1.37.36

Setting environment variables:
EMSDK = /home/ico/emsdk
EM_CONFIG = /home/ico/.emscripten
BINARYEN_ROOT = /home/ico/emsdk/clang/e1.37.36_64bit/binaryen
EMSCRIPTEN = /home/ico/emsdk/emscripten/1.37.36
```

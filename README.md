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

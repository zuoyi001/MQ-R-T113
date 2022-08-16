<p align="center">
<a href=https://twitter.com/mangopi_sbc><img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/mangopi_sbc?logo=twitter&style=flat-square"></a>

</p>

# Tina-Linux
Tina-Linux for T113/D1-H/D1s


### Ubuntu environment 
  $ sudo apt-get install build-essential subversion git-core libncurses5-dev zlib1g-dev gawk flex quilt libssl-dev xsltproc libxml-parser-perl mercurial bzr ecj cvs unzip lib32z1 lib32z1-dev lib32stdc++6 libstdc++6 libmpc-dev libgmp-dev -y

### SDK download from GitHub
``` sh
  $ git clone  https://github.com/mangopi-sbc/Tina-Linux.git
  $ cd Tina-Linux/
  $ git submodule update --init --recursive

  // download the static file
  $ wget http://dl.mangopi.cc/tina/prebuilt.tar.gz .
  $ tar xzvf prebuilt.tar.gz
  $ wget http://dl.mangopi.cc/tina/dl.tar .
  $ tar xvf dl.tar
  $ wget http://dl.mangopi.cc/tina/toolchain/riscv64-linux-x86_64-20200528.tar.xz -P ./lichee/brandy-2.0/tools/toolchain/
  $ wget http://dl.mangopi.cc/tina/toolchain/gcc-linaro-7.2.1-2017.11-x86_64_arm-linux-gnueabi.tar.xz -P ./lichee/brandy-2.0/tools/toolchain/
  
```

### Compile
  $ source build/envsetup.sh
  $ lunch
``` sh
  You're building on Linux

Lunch menu... pick a combo:
     1. d1_mq_pro-tina
     2. d1_nezha_min-tina
     3. d1_nezha-tina
     4. f133_evb1-tina
     5. f133_mq_r-tina
     6. t113_evb1-tina
     7. t113_mq_r-tina


  $ 1 or 5 or 7
  
  $ make
  $ mboot
  $ pack
  
  Tina-Linux/out/d1-mq_pro/tina_d1-mq_pro_uart0.img
  
  ``` 
  
### Flash to TF-Card

just used [phoenixcar](https://mangopi.cc/_media/phoenixcard4.2.8.zip) 

more info : https://mangopi.cc/d1 
  

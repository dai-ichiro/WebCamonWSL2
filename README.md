# WebCamonWSL2

WSL2でカメラを使うためにKernelをBuildする時に使用するconfigファイル(For Ubuntu 20.04)です。

### Ubuntu 20.04
~~~
git clone -b linux-msft-wsl-5.15.57.1 --single-branch https://github.com/microsoft/WSL2-Linux-Kernel.git
cd WSL2-Linux-Kernel
wget https://raw.githubusercontent.com/dai-ichiro/WebCamonWSL2/main/.config
sudo make -j$(nproc) && sudo make modules_install -j$(nproc) && sudo make install -j$(nproc)
~~~

### My Blog
https://touch-sp.hatenablog.com/entry/2022/01/30/001058

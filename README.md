# RTL8852BE

RTL8852BE drive installation tutorial. check network card

```
lspci | grep Network
```

## Prerequisites
```
build-essential 
gcc
bc
```

## Build(for kernel < 5.18)
```
git clone https://github.com/HRex39/rtl8852be.git
cd rtl8852be
make -j8
sudo make install
sudo modprobe 8852be
```

## Build(for kernel >= 5.18)
```
git clone https://github.com/HRex39/rtl8852be.git -b dev
cd rtl8852be
make -j8
sudo make install
sudo modprobe 8852be
```



## Reference
https://askubuntu.com/questions/1412450/network-driver-for-realtek-10ecb852

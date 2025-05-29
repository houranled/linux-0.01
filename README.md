# Linux_0.01

1)Download Source Code
https://github.com/mahadevvinay/Linux_0.01.git

2) Apply the Patch 
$cd linux
patch -p1 < 	linux_0.01_Compilations_changes.patch

3)Build the cource code
yum install libgcc.i686
yum install glibc-devel.i686
install as86 rpm package
make

4)Boot the Images  on Qemu
qemu-system-i386 -m 128M -boot a -fda Images/linux0.01-3.5.img -hdb Images/linux-0.11.img



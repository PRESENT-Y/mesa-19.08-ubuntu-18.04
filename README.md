# mesa-19.08-ubuntu-18.04


Mesa 库(libGL)静态编译

./configure

bug: configure: error: –enable-llvm is required when building r300


sudo apt-get install llvm

bug：configure: error: r600 requires libelf when using llvm

sudo apt-get install libelf-dev


make

make install 

vim ~/.zshrc

LD_LIBRARY_PATH="$MESA_INSTALLDIR/lib64" glxinfo

glxinfo |grep "OpenGL version"

OpenGL version string:3.1 Mesa 19.0.8

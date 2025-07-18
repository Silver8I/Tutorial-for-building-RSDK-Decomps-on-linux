# Tutorial-for-building-RSDK-Decomps-on-linux
The video version for this tutorial can be found [here](https://youtu.be/FKzG_SkF0VM?si=cCcQnVm_CraS4Rdq)


To install dependencies, run the following command in the command line:
```
sudo apt install build-essential cmake libglew-dev libglfw3-dev libsdl2-dev libogg-dev libtheora-dev libvorbis-dev git libgbm-dev libdrm-dev
```
To clone the source code, open a terminal in your desired folder and run one of the following commands:
```
git clone --recursive https://github.com/RSDKModding/RSDKv3-Decompilation
git clone --recursive https://github.com/RSDKModding/RSDKv4-Decompilation
git clone --recursive https://github.com/RSDKModding/RSDKv5-Decompilation
git clone --recursive https://github.com/RSDKModding/Sonic-Mania-Decompilation
```
For Sonic Forever and Sonic 2 Absolute use this command:
```
git clone --recursive https://github.com/ElspethThePict/TeamForever-v4-1.3.git
```
The Linux version is not officially supported, so please don’t ask the original developers for support.


After cloning the source code, build it into binaries by running the following commands in the terminal. (Note: This will not work for Sonic Forever or 2 Absolute; use the command below instead.)
```
cmake -B build
cmake --build build --config release
```
For Sonic Forever and Sonic 2 Absolute
```
make -j5
```
If your distro is using gcc 8.x.x then run the command below insted:
```
make -j5 LIBS=-lstdc++fs
```
You can check the gcc version your distro is using by typing this command in the terminal:
```
gcc -v
```

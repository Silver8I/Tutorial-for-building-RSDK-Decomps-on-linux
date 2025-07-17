# Tutorial-for-building-RSDK-Decomps-on-linux
The video for this can be found here [here](https://youtu.be/FKzG_SkF0VM?si=cCcQnVm_CraS4Rdq)
To install dependencies, run the following command in the command line:
```
sudo apt install build-essential cmake libglew-dev libglfw3-dev libsdl2-dev libogg-dev libtheora-dev libvorbis-dev git
```
To clone the source code, open a terminal in your desired folder and run one of the following commands:
```
git clone --recursive https://github.com/RSDKModding/RSDKv3-Decompilation
git clone --recursive https://github.com/RSDKModding/RSDKv4-Decompilation
git clone --recursive https://github.com/RSDKModding/RSDKv5-Decompilation
git clone --recursive https://github.com/RSDKModding/Sonic-Mania-Decompilation
```
After cloning the source code, build it into binaries by running the following commands in the command line:
```
cmake -B build
cmake --build build --config release
```

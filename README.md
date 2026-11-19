![License](https://img.shields.io/badge/License-GPLv3-blue.svg)

# SimpleModManager

SimpleModManager is an homebrew app for the Nintendo Switch 2 "CFW" : kaiHEN.

It will allow to manage your mods in the future (via a future implementation of LayeredFS in kaiHEN).

<p align="center"><img src="./src/Applications/SimpleModManager/resources/romfs/images/icon_corner.png" width="25%"></p>

## Screenshots

![](./screenshots/1.jpg)

<details>
  <summary><b>Spoiler: More Screenshots</b></summary>

![](./screenshots/2.jpg)
![](./screenshots/3.jpg)
![](./screenshots/4.jpg)
![](./screenshots/5.jpg)
![](./screenshots/6.jpg)

</details>


## How to install (manually)
- Download the latest version in the [release page](https://github.com/Ludwigmk/SimpleModManager-oz/releases)
- Place the .nro file in the `/switch/` folder of your SDcard.
- At the root of your SDcard, create a `/mods/` folder.
- Tree structure : `/mods/<NameOfTheGame>/<NameOfTheMod>/<ModTreeStructureFromSDcardRoot>`

Example : whatever the structure will be in the future when kaihen adds layeredfs


## Build From Source

### Prerequisites
https://github.com/ouncebrew/libounce and the following switch packages
`switch-glfw switch-glad switch-glm switch-zlib switch-freetype`

### Compile
```bash
git clone --recursive https://github.com/Ludwigmk/SimpleModManager-oz.git
cd SimpleModManager
mkdir build 
cd build
cmake ../ -DCMAKE_TOOLCHAIN_FILE=../cmake/devkita64-libnx.cmake
make
```


## Prebuilt Binaries
- To download please refer to this link : [Releases](https://github.com/Ludwigmk/SimpleModManager-oz/releases).




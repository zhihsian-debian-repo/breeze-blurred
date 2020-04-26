# BreezeBlurred
BreezeBlurred is a fork of KDE Breeze decoration.

![Screenshot](https://github.com/alex47/BreezeBlurred/blob/master/BreezeBlur_screenshot.png)
![Screenshot](https://github.com/alex47/BreezeBlurred/blob/master/BreezeBlur_screenshot3.png)
In combination with Konsole:
![Screenshot](https://github.com/alex47/BreezeBlurred/blob/master/BreezeBlur_screenshot5.PNG)

The following description is mainly copied from [SierraBreeze](https://github.com/ishovkun/SierraBreeze).


## Dependencies
There are some dependencies you'll need to install. Some people suggested using the following commands:
### Ubuntu, KDE Neon
``` shell
sudo apt install git g++ extra-cmake-modules cmake gettext libkf5config-dev libkdecorations2-dev libqt5x11extras5-dev qtdeclarative5-dev libkf5guiaddons-dev libkf5configwidgets-dev libkf5windowsystem-dev libkf5coreaddons-dev libfftw3-dev
```

### Arch Linux, Manjaro, Antergos
``` shell
sudo pacman -S kdecoration qt5-declarative qt5-x11extras kcoreaddons kguiaddons kconfigwidgets kwindowsystem fftw cmake extra-cmake-modules
```
or you can find it in the AUR: https://aur.archlinux.org/packages/breeze-blurred-git/

### OpenSUSE
``` shell
sudo zypper install git extra-cmake-modules libkdecoration2-devel kcoreaddons-devel kguiaddons-devel kconfig-devel kwindowsystem-devel ki18n-devel kconfigwidgets-devel libQt5DBus-devel libqt5-qtx11extras-devel fftw3-devel
```

## Installation
In order to install the theme and add it to your decorations do the following:
``` shell
git clone https://github.com/alex47/BreezeBlurred
cd BreezeBlurred
mkdir build
cd build
cmake .. -DCMAKE_INSTALL_PREFIX=/usr -DCMAKE_BUILD_TYPE=Release -DKDE_INSTALL_LIBDIR=lib -DBUILD_TESTING=OFF -DKDE_INSTALL_USE_QT_SYS_PATHS=ON
sudo make install
kwin_x11 --replace &
```
That is it! Your new decoration theme should appear in
*Settings &rarr; Application Style &rarr; Window Decorations*.

## Acknowledgments:
- The authors of Breeze window decorations Martin Gräßlin and Hugo Pereira Da Costa

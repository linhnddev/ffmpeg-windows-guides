Setup evironment for compiling FFmpeg on Windows plartform:

1. Install MSYS2 from https://msys2.github.io/

2. Install Mingw-W64:

pacman -S mingw-w64-x86_64-gcc

3. Install tools:

pacman -S git
pacman -S autoconf
pacman -S automake
pacman -S libtool
pacman -S make
pacman -S diffutils
pacman -S yasm
pacman -S pkg-config

4. Install required packages:

pacman -S binutils mingw-w64-x86_64-aom mingw-w64-x86_64-gnutls mingw-w64-x86_64-libbluray mingw-w64-x86_64-libvpx mingw-w64-x86_64-libass mingw-w64-x86_64-libmfx  mingw-w64-x86_64-libcdio mingw-w64-x86_64-libtheora  mingw-w64-x86_64-vo-amrwbenc mingw-w64-x86_64-libilbc mingw-w64-x86_64-libopusenc mingw-w64-x86_64-libvorbis mingw-w64-x86_64-libsoxr mingw-w64-x86_64-libxml2 mingw-w64-x86_64-dav1d mingw-w64-x86_64-x264 mingw-w64-x86_64-x265 mingw-w64-x86_64-shine mingw-w64-x86_64-ffnvcodec-headers mingw-w64-x86_64-amf-headers mingw-w64-x86_64-clang

- Above packages are required in my case. If you encourter any 'package not found' error. Try to find them in: https://packages.msys2.org/package/, install them and try again.

5. Try configure FFmpeg as normal
6. Build FFmpeg with "make" and "make install" command

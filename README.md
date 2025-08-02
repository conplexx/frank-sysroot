**diretorio gcc-arm-9.2-2019.12-x86_64-aarch64-none-linux-gnu**: cross-compilation toolchain + dependencias necessarias para gerar build linux-aarch64 do frank e evil-cinder em host linux-x86-64. gerado combinando os dois arquivos abaixo:

**gcc-arm-9.2-2019.12-x86_64-aarch64-none-linux-gnu.tar.gz**: cross-compilation toolchain oficial para Orange Pi Zero 3 com linux-aarch64 generico: http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/service-and-support/Orange-Pi-Zero-3.html (Official Tools > The cross-compilation toolchain).

**opizero3-cinder-dependencies-sysroot.tar.gz**: clone do sysroot do Orange Pi Zero3 fisico, com as dependencias de desenvolvimento para gerar build aarch64 do Cinder ja instaladas. sao elas:

- jackd2
- qjackctl
- libjack-jackd2-dev
- libxcursor-dev
- libgles2-mesa-dev
- zlib1g-dev
- libfontconfig1-dev
- libmpg123-dev
- libsndfile1
- libsndfile1-dev
- libpulse-dev
- libasound2-dev
- libcurl4-gnutls-dev
- libgstreamer1.0-dev
- libgstreamer-plugins-bad1.0-dev
- libgstreamer-plugins-base1.0-dev
- gstreamer1.0-libav
- gstreamer1.0-alsa
- gstreamer1.0-pulseaudio
- gstreamer1.0-plugins-bad
- libboost-filesystem-dev
- libxrandr-dev
- libxinerama-dev
- libxi-dev



**diretorios dos dois pacotes equivalem (e foram mergidos) de acordo com a seguinte estrutura**:

- opizero3-cinder-dependencies-sysroot.tar.gz
  - **lib**
  - **usr**

- gcc-arm-9.2-2019.12-x86_64-aarch64-none-linux-gnu.tar.gz
  - gcc-arm-9.2-2019.12-x86_64-aarch64-none-linux-gnu
    - aarch64-none-linux-gnu
      - libc
        - etc
        - **lib**
        - lib64
        - sbin
        - **usr**
        - var

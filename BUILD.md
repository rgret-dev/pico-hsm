Build instructions (tested on Debian 13):

- `apt install gcc-arm-none-eabi`
- `(git clone https://github.com/raspberrypi/pico-sdk.git && cd pico-sdk && git submodule update --init lib/tinyusb)`
- `git submodule update --init --recursive`
- `mkdir build && cd build`
- `CC=/usr/bin/gcc CXX=/usr/bin/g++ PICO_SDK_PATH=../pico-sdk cmake .. -DVIDPID=NitroHSM`
- `make`

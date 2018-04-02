cmake_minimum_required(VERSION 3.10)
project(MiniPro)

set(CMAKE_CXX_STANDARD 11)

set(CMAKE_EXE_LINKER_FLAGS "-lobjc -framework IOKit -framework CoreFoundation")

include_directories(libusb)
include_directories(libusb/os)
include_directories(src)

add_executable(MiniPro
        libusb/os/darwin_usb.c
        libusb/os/darwin_usb.h
        libusb/os/poll_posix.c
        libusb/os/poll_posix.h
        libusb/os/threads_posix.c
        libusb/os/threads_posix.h
        libusb/config.h
        libusb/core.c
        libusb/descriptor.c
        libusb/hotplug.c
        libusb/hotplug.h
        libusb/io.c
        libusb/libusb.h
        libusb/libusbi.h
        libusb/strerror.c
        libusb/sync.c
        libusb/version.h
        libusb/version_nano.h
        src/byte_utils.c
        src/byte_utils.h
        src/database.c
        src/database.h
        src/devices.h
        src/easyconfig.c
        src/easyconfig.h
        src/error.h
        src/fuses.c
        src/fuses.h
        src/main.c
        src/main.h
        src/minipro-query-db.c
        src/minipro.c
        src/minipro.h
        src/version.h)

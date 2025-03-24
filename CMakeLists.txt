cmake_minimum_required(VERSION 3.29)
project(par2cmdline)

set(CMAKE_CXX_STANDARD 23)

add_executable(par2cmdline
    src/par2cmdline.cpp
    src/commandline.cpp
    src/libpar2.cpp
    src/diskfile.cpp
    src/par2creator.cpp
    src/par2repairer.cpp
    src/par1repairer.cpp
    src/par2repairersourcefile.cpp
    src/par2creatorsourcefile.cpp
    src/creatorpacket.cpp
    src/criticalpacket.cpp
    src/reedsolomon.cpp
    src/mainpacket.cpp
    src/recoverypacket.cpp
    src/datablock.cpp
    src/md5.cpp
    src/verificationhashtable.cpp
    src/filechecksummer.cpp
    src/par1repairersourcefile.cpp
    src/par2fileformat.cpp
    src/descriptionpacket.cpp
    src/verificationpacket.cpp
    src/crc.cpp
    src/par1fileformat.cpp
)

target_compile_definitions(par2cmdline PUBLIC PACKAGE="par2cmdline")
target_compile_definitions(par2cmdline PUBLIC VERSION="0.8.1")

cmake_minimum_required(VERSION 3.7)
project(sizeVerification)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        ALL_RAID_NVRAM_Cache.cpp
        ALL_RAID_NVRAM_Cache.h
        filetable.cpp
        filetable.h)

add_executable(sizeVerification ${SOURCE_FILES})
target_link_libraries(sizeVerification pthread)
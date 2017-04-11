cmake_minimum_required(VERSION 3.1)
project(game.libretro.fbalpha2012)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR})

find_package(Kodi REQUIRED)
find_package(libretro-fbalpha2012 REQUIRED)

set(FBALPHA2012_CUSTOM_BINARY ${FBALPHA2012_LIB}
    ${PROJECT_NAME}${CMAKE_SHARED_LIBRARY_SUFFIX})

build_addon(${PROJECT_NAME} FBALPHA2012 "")

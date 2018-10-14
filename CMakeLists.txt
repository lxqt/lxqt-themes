project(lxqt-themes)
# CMP0000 - A minimum required CMake version must be specified.
# Note that the command invocation must appear in the CMakeLists.txt
# file itself; a call in an included file is not sufficient.
cmake_minimum_required(VERSION 3.6.2 FATAL_ERROR)

set(LXQTBT_MINIMUM_VERSION "0.5.0")

# lxqt-themes has no binaries - but we can set an informal version
# Version 0.13.0

find_package(lxqt-build-tools ${LXQTBT_MINIMUM_VERSION} REQUIRED)

include(GNUInstallDirs)
include(LXQtPreventInSourceBuilds)
include(LXQtTranslateDesktop)
include(LXQtConfigVars)

install(DIRECTORY "graphics/" DESTINATION "${LXQT_GRAPHICS_DIR}")
add_subdirectory(themes)
add_subdirectory(icons)

install(DIRECTORY
    .
    DESTINATION "${LXQT_SHARE_DIR}/wallpapers"
    COMPONENT Runtime
    PATTERN "CMake*"
    EXCLUDE PATTERN "cmake*"
    EXCLUDE PATTERN "Makefile" EXCLUDE
)

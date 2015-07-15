install(DIRECTORY
    .
    DESTINATION "${LXQT_SHARE_DIR}/themes"
    PATTERN "CMake*"
    EXCLUDE PATTERN "cmake*"
    EXCLUDE PATTERN "Makefile" EXCLUDE
)

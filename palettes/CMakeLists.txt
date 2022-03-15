install(DIRECTORY
    .
    DESTINATION "${LXQT_SHARE_DIR}/palettes"
    COMPONENT Runtime
    PATTERN "CMake*"
    EXCLUDE PATTERN "cmake*"
    EXCLUDE PATTERN "Makefile" EXCLUDE
)

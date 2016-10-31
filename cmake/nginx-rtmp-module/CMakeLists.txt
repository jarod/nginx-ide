set(PROJ_DIR "${ROOT_DIR}/nginx-rtmp-module")
file(GLOB_RECURSE SRCS "${PROJ_DIR}/*.c")
add_library(nginx-rtmp-module STATIC "${SRCS}")

set(PROJ_DIR "${ROOT_DIR}/nginx")
file(GLOB_RECURSE SRCS "${PROJ_DIR}/*.c")
include_directories("${INCLUDE_DIRECTORIES}
    ${PROJ_DIR}/src/core"
    ${PROJ_DIR}/src/event"
    ${PROJ_DIR}/src/http"
    ${PROJ_DIR}/src/mail"
    ${PROJ_DIR}/src/misc"
    ${PROJ_DIR}/src/os"
    ${PROJ_DIR}/src/stream"
)
add_executable(nginx "${SRCS}")

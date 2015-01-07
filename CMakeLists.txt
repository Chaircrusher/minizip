project(minizip)

set(zip_SRCS zip.c unzip.c ioapi.c)

add_library(zip ${zip_SRCS})

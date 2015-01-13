cmake_minimum_required(VERSION 2.8)
project(minizip)

set(zip_SRCS zip.c unzip.c ioapi.c)

add_library(zip ${zip_SRCS})

install(TARGETS zip
  RUNTIME DESTINATION bin
  LIBRARY DESTINATION lib
  ARCHIVE DESTINATION lib
)
INSTALL(FILES zip.h ioapi.h unzip.h
  DESTINATION include
)

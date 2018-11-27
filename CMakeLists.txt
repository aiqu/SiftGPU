CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(SIFTGPU C CXX)

SET(WARN_FLAGS "-Wno-int-to-pointer-cast -Wno-maybe-uninitialized -Wno-unused-but-set-variable -Wno-write-strings -Wno-unused-result -Wno-deprecated -fPIC")
SET(CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} ${WARN_FLAGS}")
SET(CMAKE_C_FLAGS  "${CMAKE_C_FLAGS} ${WARN_FLAGS}")

ADD_SUBDIRECTORY(src)


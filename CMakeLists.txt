cmake_minimum_required(VERSION 3.16)

project(
  cpm-magical-test
  VERSION 1.0
  LANGUAGES C
)

add_library(magiclib src/magic.c)

target_include_directories(magiclib PUBLIC
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
  $<INSTALL_INTERFACE:include>  # <prefix>/include
)

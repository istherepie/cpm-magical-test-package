cmake_minimum_required(VERSION 3.16)

project(
  cpm-magical-test
  VERSION 1.0
  LANGUAGES C
)

add_library(magiclib src/magic.c src/magic.h)

include_directories (.)

cmake_minimum_required (VERSION 2.6)

project (libgvps)

# TODO add linux only  -Ofast -std=c99 -Wall -fPIC

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -DFP_TYPE=float")

add_library(libgvps gvps_sampled.c gvps_full.c gvps_variable.c gvps_obsrv.c)

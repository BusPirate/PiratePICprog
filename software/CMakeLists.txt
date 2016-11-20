cmake_minimum_required(VERSION 3.5 FATAL_ERROR)
project(picprog)
set (PICPROG_SOURCE_FILES buspirate.c common.c data_file.c debug.c iface.c
  main.c memory.c pic.c pic12.c pic16.c pic18.c pic24.c pic32.c proto_pic.c
  serial.c)
add_executable (picprog ${PICPROG_SOURCE_FILES})

set (COMPARE_SOURCE_FILES common.c compare.c data_file.c debug.c memory.c)
add_executable (compare ${COMPARE_SOURCE_FILES})

# vim:sts=2:sw=2:ts=2:et:syn=cmake:fdm=marker:ff=unix:fenc=utf8:number:cc=80

cmake_minimum_required (VERSION 3.19)

include(pico_sdk_import.cmake)

project(blink_sobhit_project)

pico_sdk_init()

#This creates an executable target "blink" from a single source file blink.c
add_executable(blink blink.c)


#Generates different file formats such as .uf2 .elf .bin
pico_add_extra_outputs(blink)

#Specifies libraries - flags to use when linking a given target
target_link_libraries(blink pico_stdlib)








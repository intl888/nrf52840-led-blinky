cmake_minimum_required(VERSION 3.20.0)
set(BOARD nrf52840dk_nrf52840)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(led_blinky_project)

target_sources(app PRIVATE src/main.c)
set(CMAKE_BUILD_TYPE Debug)
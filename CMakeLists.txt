cmake_minimum_required(VERSION 3.5)

set(ElegantOTA_SRCS
  src/ElegantOTA.cpp
  src/elop.cpp
  )

idf_component_register(SRCS ${ElegantOTA_SRCS}
                       INCLUDE_DIRS "src"
                       REQUIRES arduino-esp32)

project(ElegantOTA)
add_library(pico_mpr121 INTERFACE)

target_include_directories(pico_mpr121 INTERFACE 
  ${CMAKE_CURRENT_LIST_DIR}
)

target_link_libraries(pico_mpr121 INTERFACE
  hardware_i2c
)

target_sources(pico_mpr121 INTERFACE
  ${CMAKE_CURRENT_LIST_DIR}/mpr121.c
)

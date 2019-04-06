project(osvcorerun)

include_directories(../unixcoreruncommon)

add_compile_options(-fPIC)

add_library_clr(osvcorerun
  SHARED
  corerun.cpp
)

target_link_libraries(osvcorerun
    unixcoreruncommon
)

install_clr(osvcorerun)

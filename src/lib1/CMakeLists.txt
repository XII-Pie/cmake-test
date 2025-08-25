
add_library(lib1 lib1.cc)

target_include_directories(lib1 PUBLIC .)

set_target_properties(lib1 PROPERTIES 
    PUBLIC_HEADER "lib1.h"
)

install(TARGETS lib1
    LIBRARY DESTINATION lib
    PUBLIC_HEADER DESTINATION include
)


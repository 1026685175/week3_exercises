# add Library Automata_Lib

add_library(Automata_lib automaton.cpp) # add library
target_include_directories(Automata_lib PUBLIC ${CMAKE_SOURCE_DIR}/include) # add include directory


# add executable 

add_executable(Automata_example main.cpp) # add executable
target_link_libraries(Automata_example PUBLIC Automata_lib) # link library to executable
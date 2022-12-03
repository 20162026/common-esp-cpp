cmake_minimum_required(VERSION 3.5)

set(srcs "pl_mutex.cpp" "pl_lock_guard.cpp" "pl_buffer.cpp" "pl_stream.cpp" "pl_hardware_interface.cpp" "pl_server.cpp")
add_prefix(srcs "${CMAKE_CURRENT_LIST_DIR}/" ${srcs})

idf_component_register( SRCS ${srcs}
                        INCLUDE_DIRS "include")
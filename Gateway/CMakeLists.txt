# The following lines of boilerplate have to be in your project's
# CMakeLists in this exact order for cmake to work correctly
cmake_minimum_required(VERSION 3.5)

include($ENV{IDF_PATH}/tools/cmake/project.cmake)

set(EXTRA_COMPONENT_DIRS 
    ${CMAKE_CURRENT_LIST_DIR}/components/http_server_app
    ${CMAKE_CURRENT_LIST_DIR}/components/lora
    $ENV{IDF_PATH}/examples/common_components/protocol_examples_common)


project(Project2)
# Add binary data to the target
target_add_binary_data(${CMAKE_PROJECT_NAME}.elf "html/index.html" TEXT)

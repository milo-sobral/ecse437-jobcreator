# MUST BE PLACED: src/utils/CMakeLists.txt

# Set the project name
project (utils)

# Add a library with the above sources
add_library(${PROJECT_NAME} ${PROJECT_SOURCE_DIR}/input.c)

target_include_directories( ${PROJECT_NAME}
    PUBLIC ${PROJECT_SOURCE_DIR}/../include
)

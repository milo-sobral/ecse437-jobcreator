# MUST BE PLACED: src/jobs/CMakeLists.txt

# Set the project name
project (jobs)

# Add a library with the above sources
add_library(${PROJECT_NAME} ${PROJECT_SOURCE_DIR}/job.c)

target_include_directories( ${PROJECT_NAME}
    PUBLIC ${PROJECT_SOURCE_DIR}/../include
)

cmake_minimum_required(VERSION 3.10)

# set the project name
project(jobcreator)

# Add sub directories
add_subdirectory(utils)
add_subdirectory(jobs)

# add the executable
add_executable(jobcreator main.c)

target_include_directories( ${PROJECT_NAME}
    PUBLIC ${PROJECT_SOURCE_DIR}/include
)

target_link_libraries(${PROJECT_NAME}
    utils
    jobs
)

install(TARGETS jobcreator DESTINATION bin)

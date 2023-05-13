cmake_minimum_required(VERSION 3.15)
project(project-starter)

find_package(CLI11 2.3.2 REQUIRED)
find_package(nlohmann_json 3.11.2 REQUIRED)

add_executable(${PROJECT_NAME} src/main.cpp)
target_link_libraries(${PROJECT_NAME}
    CLI11::CLI11
    nlohmann_json::nlohmann_json
)
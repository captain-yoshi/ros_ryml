cmake_minimum_required(VERSION 3.12)
project(ryml)

find_package(catkin REQUIRED)

catkin_package(
  LIBRARIES
    ${PROJECT_NAME}
  INCLUDE_DIRS
    rapidyaml/src
    rapidyaml/ext/c4core/src
)

# Cloned from:
# https://github.com/biojppm/rapidyaml/commit/ff5493188293eab30f1294241461abebe29e56fa
add_subdirectory(rapidyaml)

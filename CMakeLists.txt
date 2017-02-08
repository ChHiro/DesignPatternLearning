project(DesignPatternQuiz)
cmake_minimum_required(VERSION 3.0)
find_package(Qt5Widgets REQUIRED)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS -Wall)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(DPQ_SOURCES

    )
set(DPQ_UI_SOURCES
    main.cpp
    #mainwindow.ui
    #mainwindow.cpp
    )


#aux_source_directory(. SRC_LIST)
add_executable(${PROJECT_NAME} ${DPQ_SOURCES} ${DPQ_UI_SOURCES} ${HEADERS})
QT5_USE_MODULES(${PROJECT_NAME} Widgets)

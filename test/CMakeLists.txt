find_package(OpenCV REQUIRED)

include_directories(
  ${OpenCV_INCLUDE_DIRS}
)

link_directories(
  ${OpenCV_LIBRARY_DIRS}
)

add_executable(test_edline_detector test_edline_detector.cpp)
target_link_libraries(test_edline_detector EDLine ${OpenCV_LIBS})


cmake_minimum_required(VERSION 2.8)
project( DenseTrackStab )
find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} include/ )
add_executable( DenseTrackStab src/DenseTrackStab.cpp )
target_link_libraries( DenseTrackStab ${OpenCV_LIBS} )

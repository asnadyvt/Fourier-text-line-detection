cmake_minimum_required(VERSION 2.8)
project( Ex3 )

#
find_package( OpenCV REQUIRED )

#
add_executable( Ex3
	util.cpp
	ex3.cpp
)

target_include_directories( Ex3
	PRIVATE .
          ${OpenCV_INCLUDE_DIRS}
)

target_link_libraries( Ex3
	${OpenCV_LIBS} 
)

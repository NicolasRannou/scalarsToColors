cmake_minimum_required(VERSION 2.6)
 
PROJECT(ScalarToColor)
 
FIND_PACKAGE(VTK REQUIRED)
INCLUDE(${VTK_USE_FILE})
 
ADD_EXECUTABLE(ScalarToColor ScalarToColor.cxx)
TARGET_LINK_LIBRARIES(ScalarToColor vtkHybrid vtkInfovis)

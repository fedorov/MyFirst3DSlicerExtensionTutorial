cmake_minimum_required(VERSION 2.8.9)

project(MyFirstSlicerExtension)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/fedorov/MyFirstSlicerExtension")
set(EXTENSION_CATEGORY "Learning")
set(EXTENSION_CONTRIBUTORS "Andrey Fedorov (BWH)")
set(EXTENSION_DESCRIPTION "This extension is developed as part of Slicer extension writing tutorial")
set(EXTENSION_ICONURL "https://raw.github.com/fedorov/MyFirstSlicerExtension/master/MyFirstSlicerExtension.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MyFirstSlicerExtension/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})

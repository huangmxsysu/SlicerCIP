cmake_minimum_required(VERSION 3.0.1)

project(SlicerCIP)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_NAME "SlicerCIP")
set(EXTENSION_HOMEPAGE "http://www.slicer.org/slicerWiki/index.php/Documentation/4.3/Extensions/OpenCAD")
set(EXTENSION_CATEGORY "Chest Imaging Platform")
set(EXTENSION_CONTRIBUTORS "Raul San Jose (BWH)")
set(EXTENSION_DESCRIPTION "Slicer Chest Imaging Platform provides Chest CT quantification tools for lung diseases including COPD and Lung Cancer")
set(EXTENSION_ICONURL "")
set(EXTENSION_SCREENSHOTURLS "")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LesionSizing)
#add_subdirectory(LungDensitometry)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
cmake_minimum_required(VERSION 3.13.4)

project(MIP_Assignment)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/MIP_Assignment")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "Kaushalya (UoM)")
set(EXTENSION_DESCRIPTION "“Line intensity profile” plots intensity levels of pixels within a drawn line. Line intensity profile can 
compare the noise levels of multiple images and compare physical properties of anatomical structures ")
set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/MIP_Assignment.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MIP_Assignment/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})

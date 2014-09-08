INCLUDE_DIRECTORIES(../include)

#slicerMacroBuildCLI(
SEMMacroBuildCLI (
  NAME LesionSegmentation
  TARGET_LIBRARIES ${ITK_LIBRARIES}
  EXECUTABLE_ONLY
  )
if(BUILD_TESTING)
  add_subdirectory(Testing)
endif()

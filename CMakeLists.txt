project(lib_WFpropagate_project)

include_directories ("${PROJECT_SOURCE_DIR}/src")
include_directories ("${PROJECT_SOURCE_DIR}/..")

add_library(WFpropagate SHARED WFpropagate.c 
	WFpropagate.h
)

install(TARGETS WFpropagate DESTINATION lib)
install(FILES WFpropagate.h DESTINATION include)


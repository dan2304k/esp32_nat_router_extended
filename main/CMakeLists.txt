FILE(GLOB_RECURSE app_sources ${CMAKE_SOURCE_DIR}/main/*)

idf_component_register(SRCS ${app_sources} INCLUDE_DIRS ".")

message(STATUS "app_sources ${app_sources}")

target_add_binary_data(${COMPONENT_TARGET} "pages/favicon.ico" BINARY)
target_add_binary_data(${COMPONENT_TARGET} "pages/styles-9ee3c4491d35b3c1d830fa9da31c7861.css" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/config.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/result.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/apply.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/scan.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/reset.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/unlock.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/advanced.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/lock.html" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/jquery.js" TEXT)
target_add_binary_data(${COMPONENT_TARGET} "pages/bootstrap.js" TEXT)

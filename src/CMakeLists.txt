project(planning_main)

#Ìí¼Ó×ÓÄ¿Â¼
add_subdirectory(pnc_map)
add_subdirectory(process)

add_executable(${PROJECT_NAME} planning_main.cpp)

target_include_directories(${PROJECT_NAME}
PUBLIC
${Process_Dir}
)

target_link_libraries(${PROJECT_NAME}
PUBLIC
process
)





add_subdirectory(minhook)
add_subdirectory(imgui)

target_link_libraries(grounded_minimap PRIVATE minhook)
target_include_directories(grounded_minimap PRIVATE minhook/include)

target_link_libraries(grounded_minimap PRIVATE imgui imgui_backends)
target_include_directories(grounded_minimap PRIVATE imgui)

target_include_directories(grounded_minimap PRIVATE stb_image)

target_include_directories(grounded_minimap PRIVATE tomlplusplus)
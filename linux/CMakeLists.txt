add_executable(ButtonMash_Linux
	main.cpp
)

target_link_libraries(ButtonMash_Linux PRIVATE
	sfml-graphics
	sfml-window
	sfml-system
)
target_link_libraries(ButtonMash_Linux PUBLIC
	ButtonMashLib
)

target_include_directories(ButtonMash_Linux PUBLIC
                          "${PROJECT_BINARY_DIR}"
                          "${PROJECT_SOURCE_DIR}/core"
                          )

target_compile_features(ButtonMash_Linux PRIVATE cxx_std_17)
add_library(${EXEC_NAME}_CMSIS EXCLUDE_FROM_ALL
	GD/GD32F30x/Source/GCC/startup_gd32f30x_hd.S
	GD/GD32F30x/Source/system_gd32f30x.c
)

target_include_directories(${EXEC_NAME}_CMSIS PUBLIC
	.
	GD/GD32F30x/Include
)

target_link_libraries(${EXEC_NAME}_CMSIS ${EXEC_NAME}_standard_peripherals)
add_library(${EXEC_NAME}_gd32f307c_eval EXCLUDE_FROM_ALL
gd32f307c_eval.c
)

target_include_directories(${EXEC_NAME}_gd32f307c_eval PUBLIC
	.
)

target_link_libraries(${EXEC_NAME}_gd32f307c_eval ${EXEC_NAME}_CMSIS)

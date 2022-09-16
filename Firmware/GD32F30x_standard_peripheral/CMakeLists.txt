add_library(
  ${EXEC_NAME}_standard_peripherals EXCLUDE_FROM_ALL
  Source/gd32f30x_adc.c
  Source/gd32f30x_crc.c
  Source/gd32f30x_dbg.c
  Source/gd32f30x_exmc.c
  Source/gd32f30x_fwdgt.c
  Source/gd32f30x_misc.c
  Source/gd32f30x_rtc.c
  Source/gd32f30x_timer.c
  Source/gd32f30x_bkp.c
  Source/gd32f30x_ctc.c
  Source/gd32f30x_dma.c
  Source/gd32f30x_exti.c
  Source/gd32f30x_gpio.c
  Source/gd32f30x_pmu.c
  Source/gd32f30x_sdio.c
  Source/gd32f30x_usart.c
  Source/gd32f30x_can.c
  Source/gd32f30x_dac.c
  Source/gd32f30x_enet.c
  Source/gd32f30x_fmc.c
  Source/gd32f30x_i2c.c
  Source/gd32f30x_rcu.c
  Source/gd32f30x_spi.c
  Source/gd32f30x_wwdgt.c)

target_include_directories(${EXEC_NAME}_standard_peripherals PUBLIC Include)

target_link_libraries(${EXEC_NAME}_standard_peripherals ${EXEC_NAME}_CMSIS)

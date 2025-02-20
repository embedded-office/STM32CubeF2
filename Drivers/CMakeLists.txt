#******************************************************************************
#   Copyright 2020 Embedded Office GmbH & Co. KG
#
#   Licensed under the Apache License, Version 2.0 (the "License");
#   you may not use this file except in compliance with the License.
#   You may obtain a copy of the License at
#
#       http://www.apache.org/licenses/LICENSE-2.0
#
#   Unless required by applicable law or agreed to in writing, software
#   distributed under the License is distributed on an "AS IS" BASIS,
#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#   See the License for the specific language governing permissions and
#   limitations under the License.
#******************************************************************************

add_library(stm32f2xx-hal)

target_sources(stm32f2xx-hal
  PRIVATE
    STM32F2xx_HAL_Driver/Src/Legacy/stm32f2xx_hal_can.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_adc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_adc_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_can.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_cortex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_crc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_cryp.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_dac.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_dac_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_dcmi.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_dcmi_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_dma.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_dma_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_eth.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_exti.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_flash.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_flash_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_gpio.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_hash.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_hcd.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_i2c.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_i2s.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_irda.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_iwdg.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_mmc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_msp_template.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_nand.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_nor.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_pccard.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_pcd.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_pcd_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_pwr.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_pwr_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_rcc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_rcc_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_rng.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_rtc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_rtc_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_sd.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_smartcard.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_spi.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_sram.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_tim.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_timebase_rtc_alarm_template.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_timebase_rtc_wakeup_template.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_timebase_tim_template.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_tim_ex.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_uart.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_usart.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_hal_wwdg.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_adc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_crc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_dac.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_dma.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_exti.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_fsmc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_gpio.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_i2c.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_pwr.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_rcc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_rng.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_rtc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_sdmmc.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_spi.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_tim.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_usart.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_usb.c
    STM32F2xx_HAL_Driver/Src/stm32f2xx_ll_utils.c    
)

target_include_directories(stm32f2xx-hal
  PUBLIC
    CMSIS/Include
    CMSIS/Device/ST/STM32F2xx/Include
    STM32F2xx_HAL_Driver/Inc
    STM32F2xx_HAL_Driver/Inc/Legacy
    ${STM_HAL_CONF_DIR}
)

if (${STM_USE_HAL_DRIVER})
  target_compile_definitions(stm32f2xx-hal PUBLIC USE_HAL_DRIVER)
endif()
if (${STM_USE_FULL_LL_DRIVER})
  target_compile_definitions(stm32f2xx-hal PUBLIC USE_FULL_LL_DRIVER)
endif()
if (${STM_USE_FULL_ASSERT})
  target_compile_definitions(stm32f2xx-hal PUBLIC USE_FULL_ASSERT)
endif()
target_compile_definitions(stm32f2xx-hal PUBLIC ${STM_HAL_DEVICE})

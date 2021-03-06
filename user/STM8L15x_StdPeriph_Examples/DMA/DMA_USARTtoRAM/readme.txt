/** @page DMA_USARTtoRAM Use DMA to transfer continuously data received by USART to RAM with (data real time display on LCD)

  @verbatim
  ******************** (C) COPYRIGHT 2013 STMicroelectronics *******************
  * @file    DMA/DMA_USARTtoRAM/readme.txt 
  * @author  MCD Application Team
  * @version V1.5.2
  * @date    30-September-2014
  * @brief   Description of the DMA's USART to RAM example.
  ******************************************************************************
  *
  * Licensed under MCD-ST Liberty SW License Agreement V2, (the "License");
  * You may not use this file except in compliance with the License.
  * You may obtain a copy of the License at:
  *
  *        http://www.st.com/software_license_agreement_liberty_v2
  *
  * Unless required by applicable law or agreed to in writing, software 
  * distributed under the License is distributed on an "AS IS" BASIS, 
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  ******************************************************************************
   @endverbatim

  @par Example description

  This example provides a short description of how to use the DMA peripheral in 
  circular mode to transfer data from USART peripheral to RAM memory.
  When the user sends a character using USART, this character will be 
  transferred using DMA to a specific RAM Table.
  As this RAM Table content is indefinitely displayed on LCD, any character 
  written in the HyperTerminal will be displayed instantly on LCD.
  
  @par Directory contents

  - DMA/DMA_USARTtoRAM/main.c             Main file containing the "main" function
  - DMA/DMA_USARTtoRAM/stm8l15x_conf.h    Library Configuration file
  - DMA/DMA_USARTtoRAM/stm8l15x_it.c      Interrupt routines source
  - DMA/DMA_USARTtoRAM/stm8l15x_it.h      Interrupt routines declaration

  @par Hardware and Software environment

    - This example runs on STM8L15x High-Density, Medium-Density Plus, Medium-Density
    and Low-Density Devices.
  
  - This example has been tested with STMicroelectronics STM8L1528-EVAL 
    (STM8L15x High-Density devices) and STM8L1526-EVAL (STM8L15x Medium-Density and
    Low-Density devices) evaluation boards and can be easily tailored to any other
    development board.

  - STM8L1528-EVAL Set-up 
    - Make sure that the LCD glass daughter board is mounted in IO position.
      For more details please refer to the evaluation board user manual.
    - Connect a null-modem female/female RS232 cable between the DB9 connector 
      CN7 and PC serial port.
    - Make sure that JP5 jumper is in RS232 position
    - Make sure that JP11 jumper is in RS232 position    
    - Dot matrix LCD
        
  - STM8L1526-EVAL Set-up
     - Make sure that the LCD glass daughter board is mounted in IO position.
      For more details please refer to the evaluation board user manual.
     - Connect a null-modem female/female RS232 cable between the DB9 connector 
       CN1 and PC serial port.
     - Make sure that JP5 jumper is in RS232 position
     - Dot matrix LCD
      
  - HyperTerminal configuration:
    - Word Length = 8 Bits
    - One Stop Bit
    - No parity
    - BaudRate = 115200 baud
    

  @par How to use it ?

  In order to make the program work, you must do the following :

  - Copy all source files from this example folder to the template folder under
    Project\STM8L15x_StdPeriph_Template
  - Open your preferred toolchain 
  - Add the required files :
    - stm8_eval.c   (under Utilities\STM8_EVAL)
    - stm8_eval_lcd.c   (under Utilities\STM8_EVAL\Common)
  - Rebuild all files and load your image into target memory
  - Run the example 
  - Write any text on HyperTerminal, it will be displayed instantly on LCD.
  


 * <h3><center>&copy; COPYRIGHT STMicroelectronics</center></h3>
 */

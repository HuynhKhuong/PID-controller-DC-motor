# Hardware items list for project DC Motor controller via PID 

## Item list 

| Item| Name  | Description |  
| ----- | -------- | ----- |
| MCU | STM32F103C8T6| - FPU <br> - CLK 80MHz – 500MHz  <br> required peripherals:<br> - 1 timer PWM.<br> - 1 timer to schedule calculation <br> - General Purpose Oupun <br> - General Purpose Input/timen <br> - UART |
| DC motor | GM25-370| - VDC: 12VDC <br> - Encoder: 2 channels A, B. resolution: 11 pulses/1 channel/ 1 round. <br> - transmit ratio 34:1. <br> - Output resolution: 11 x 34 = 374 pulse/channel/round. <br> - Encoder Supply voltage: 3.3~5VDC <br> - consumed current without load: 150mA <br> - Max consumed current: 750mA <br> - Speed (no load): 250 RPM  <br> - Maximum Speed: 140 RPM <br> - Moment: 4.3 Kg.cm <br> - Maximum Moment: 5.2 Kg.cm|
| H-bridge | L298 |- Dual Full Bridge Driver <br> - VDC 5~30VDC; Max consumed current (each channel): 2A; <br> - maxed consumed power: 25W (each channel)|

## Hardware setup

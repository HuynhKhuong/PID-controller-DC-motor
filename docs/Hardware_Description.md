# Hardware items list for project DC Motor controller via PID 

## Item list 

| Item| Name  | Description |  
| ----- | -------- | ----- |
| MCU | STM32F103C8T6| - FPU \n - CLK 80MHz – 500MHz  \n required peripherals:\n 1 timer PWM.\n 1 timer to schedule calculation \n General Purpose Oupun \n General Purpose Input/timen \n UART |
| DC motor | GM25-370| - VDC: 12VDC \n Encoder: 2 channels A, B. resolution: 11 pulses/1 channel/ 1 round. \n transmit ratio 34:1. \n Output resolution: 11 x 34 = 374 pulse/channel/round. \n Encoder Supply voltage: 3.3~5VDC \n consumed current without load: 150mA \n Max consumed current: 750mA \n Speed (no load): 250 RPM  \n Maximum Speed: 140 RPM \n Moment: 4.3 Kg.cm \n Maximum Moment: 5.2 Kg.cm|
| H-bridge | L298 |- Dual Full Bridge Driver \n VDC 5~30VDC; Max consumed current (each channel): 2A; \n maxed consumed power: 25W (each channel)|

## Hardware setup

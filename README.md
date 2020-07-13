# DMA-based LED dimming
This example uses DMA to move the reading from the ADC to PWM duty-cycle in the background without CPU intervention.

# Description
This example demonstrates the usage of DMA. It uses DMA to move data from the ADC result register to the PWM duty-cycle registers. The DMA is capable of moving one segment of data to multiple memory locations. Therefore, the ADC reads the voltage level from the POT on Curiosity HPC and the DMA is able to feed this data to three PWMs with different frequencies.
![](https://static.transim.com/img/82018/94efb50d2ad0459ab43736cf99eeba0f-4nbl2.png){width=auto height=auto align=center}

# Result
As you turn the POT, you can see the LEDs flashing at different frequencies, but change with the same intensity.

This example is used in the livestream "Think Outside the CPU: MCU Signal Processing Without Using the Core". Check out [the livestream](https://www.youtube.com/watch?v=MK0ci7FHcdc&feature=youtu.be) for more information.
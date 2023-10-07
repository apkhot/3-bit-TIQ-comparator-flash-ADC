# 3-bit-TIQ-comparator-flash-ADC
A Three-Bit Threshold Inverter Quantization Based CMOS Flash ADC 

There are various types of ADCs. Among these, four types of architecture are the most popular. These are flash, pipelined, sigma-delta, and successive approximation register (SAR). Flash ADCs are the fastest among all other types for their parallel architectures. Typical flash ADC utilizing a resistor ladder requires 2n-1 comparators for an n-bit ADC. For example, a 3-bit ADC requires 7 comparators.  Each comparator has a reference voltage which is usually given from external reference voltage. Analog voltage is connected to all the comparators so that conversions occur in parallel. The comparators produce logic ‘1’ for which the analog voltage is larger than the reference input. Because of using a resistor ladder, these typical flash ADCs are power-hungry and space-consuming. A TIQ-based ADC chip is comprised of three basic blocks. These blocks are the TIQ comparator, gain booster, and thermometer to the binary encoder. The TIQ technique uses two cascaded CMOS inverters as a comparator. While the second inverter serves as a gain booster, the first inverter internally creates reference voltage (Vref). As we adjust the size of CMOS, the cascading inverters produce various switching/reference voltages internally which serve as reference voltages. 

Schematic:

![image](https://github.com/apkhot/3-bit-TIQ-comparator-flash-ADC/assets/47900640/35293a24-1a4f-4d16-82f6-1e3854647239)

Two inverters are linked in series on the TIQ Comparator for comparing and balancing. The threshold voltage of the inverter circuits can be modified to provide different reference voltages by adjusting the width of PMOS and NMOS transistors. In analog section of 3-bit ADC, comparators that is, 7 TIQ comparators are connected parallelly using CMOS inverters. Where, n is the number of output binary bits.

Simulation Plot:

![image](https://github.com/apkhot/3-bit-TIQ-comparator-flash-ADC/assets/47900640/2ee95036-0ed7-408c-9ab8-0cfe9060715d)

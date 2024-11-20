# FreeRTOS on Ti-F280049C DSP

This is a freertos prototype on F280049C. The key setting is the memory layout setting in the .cmd file. Added stacks and heaps for use by freertos.

```c
   .freertosStaticStack  : >> RAMM1 | RAMLS5 | RAMLS6,     PAGE = 1
   .freertosHeap         : >> RAMGS0 | RAMGS1 | RAMGS2,     PAGE = 1
```
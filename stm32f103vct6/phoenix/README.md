STM32芯片项目学习记录
[toc]
### 1、LED点灯程序
### 2、printf打印的内容重定向到usart1串口
    1.先通过stm32cubemax配置好usart1
    2.通过重写函数fputc函数（c语言printf函数会使用fputc去put字符），使用HAL_UART_Transmit去重定向一下。
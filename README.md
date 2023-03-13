# M480BSP_UART4_Tx_PDMA
 M480BSP_UART4_Tx_PDMA


update @ 2023/03/13

1. initial UART4 TX (PC.7) w/ PDMA function 

- with 2 define ENALBE_PDMA_IRQ ,  ENALBE_PDMA_POLLING , for PDMA transfer function

2. TX Buffer length set as 32 , send TX buffer per 500 ms , 

- set buffer index 0 , 1 as 0x5A , for indicator

- set buffer last index n-1 , n-2 , as 0x A5 , for indicator

- set buffer last index n-3 , as a counter (increase per 500ms) , for indicator

3. below is LA capture  , 

below is buffer transmit timing 

![image](https://github.com/released/M480BSP_UART4_Tx_PDMA/blob/main/LA.jpg)	



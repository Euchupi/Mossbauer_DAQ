# Mossbauer Data Splitter 

A firmware written in verilog for RedPitaya STMLab 125-14 , compiled in Vivado 2020.1 . 

if running on old operating system of redpitaya :

` fpgautil -b systemwrapper.bit.bin 

else if running on new operating system of redpitaya , 



Register Map (GPIO)
| GPIO | Length | Offset | Description |
| -- |  -- | --|  --  | 
| 0 | 32bit | 0x42000000 | 0~15 Ch1 , 16~31 Ch2 Lastest Data | 
| 1 | 32bit | 0x42100000 | 0~15 Smoothed CH1 Data | 
| 2 | 32bit | 0x42200000 | 0~15 Low Threshold, 16~31 High Threshold | 
| 3 | 32bit | 0x42300000 | 0~31 Slow Clock Counts | 
| 4 | 32bit | 0x42400000 | 0~31 Enable Duration | 
| 5 | 32bit | 0x42500000 | Unused | 



Interaction Section is to automatically set the parameters is under developping. 

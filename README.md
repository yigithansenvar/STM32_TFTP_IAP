# STM32_TFTP_IAP
In this project, I did an embedded system software update using TFTP.
The IAP checks whether there is a new software update when the system is reset or operated by the user with an effect.
If there is a new update, it will download and run the new software. IAP codes write new application codes in the Flash memory area if you have a new update request. 
In this project, IAP codes were written on the first pages of flash memory. Application codes were written on the rest of the flash memory. Thus, when the microcontroller is reset,
the IAP program first works. The task of Iap codes will be downloaded and write the memory allocated for the application. Then, if the downloaded file is correctly written in flash memory,
Iap application will be switched to the new downloaded application. If the application codes have not been downloaded correctly, IAP codes will continue to operate.

YOUTUBE VIDEO: https://youtu.be/7kUgk6nNf98

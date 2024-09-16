
# Introduction
OW devices are machines that release scents. The device has 6 scent channels which contain scents that can be released. Your task will be to design and write code to control the scent delivery device.

# System Overview
## Scent delivery device description
The scent delivery device has 6 channels. To open a channel and release a scent, a corresponding air control valve needs to be opened and a diaphragm pump started.

To open a valve, the GPIO pin on a microcontroller needs to be set to high. To close a valve, the GPIO pin needs to be set to low.
The valve GPIO pin mapping is as follows:

| Channel | GPIO |
|---------|------|
| 1       | 46   |
| 2       | 3    |
| 3       | 8    |
| 4       | 18   |
| 5       | 17   |
| 6       | 16   |


The pump is controlled by GPIO pin 11. To start the pump, the GPIO pin needs to be set high. To stop the pump, the GPIO pin needs to be set low.

## Communication
Serial communication is used to send and receive messages to and from the device.

# Requirements
Develop code for an embedded system that will enable the controlled release of scents (for a specific channel). Commands should be sent via serial communication and should specify the channel to open. The channel will stay open for 60 seconds and then close again.

# Instructions
1. Using the information and requirements above, design and code a solution that will fulfill the requirements.
2. Include a README file that explains your design process assumptions and any other information you think is relevant. 
3. README should also include instructions on how you would run your test or code if appropriate.

# Criteria
1. You should not spend more than 2 hours on this task. We are not looking for a complete solution, but rather a demonstration of your thought process and how you approach a problem. 
2. The code should be written in C/C++. 
3. You can mock the pin and serial communication in your code.
4. Explain your process in the interview. The goal of this exercise is to understand your design process, and how you think about the implementation of the requirements. 

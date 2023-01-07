- 👋 **Group Name:** Learning Leopards
- 👀 **Group Members:** Deveepria A/P Sankaran, Nur Irdina binti Mohd Shahrir, Thulasy A/P Chandran
- 🌱 **Task description:-** We explore a keyword-based spoken language understanding system, in which the intent of the user can directly be derived from the detection of a sequence of keywords in the query. We focus on the keyword spotting method and edge impulse which is the leading development platform for machine learning on edge devices and free for developers. Edge impulse is used to perform audio data classification.

As we continue the series with STM32, let’s take a look at how to use the analog-to-digital converter (ADC). At first, we set up a single conversion that samples the voltage from a potentiometer and transmits the raw value over UART. We can then read this information on a serial terminal.

We run into problems, however, when we want to sample analog voltages at a much faster rate. So, we introduce the concept of direct memory access (DMA) to help pipe data from the ADC (or any other peripheral) to memory.

We can also use the DMA controller the other way, too. We start by showing an example of reading a large buffer of test data out over UART via DMA. From there, we build a quick demo of filling a circular buffer with ADC readings with the DMA controller. We’ll simply peek at the buffer contents in the STM32CubeIDE debugger to show how the DMA can act without CPU intervention.


- 💞️ **Youtube:** 
- 📫 **References:** Lecture Note, Chapter 10: Serial Interfacing https://www.hackster.io/ashish205/stm32f0-push-button-to-switch-on-led-bc9958 https://www.engineersgarage.com/insight-how-dip-switch-works/ https://www.youtube.com/watch?v=JZsC34jfbEg https://microcontrollerslab.com/push-button-control-leds-stm32f4-discovery-board-digital-input-pins-hal-driver/

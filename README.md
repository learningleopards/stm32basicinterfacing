- 👋 **Group Name:** Learning Leopards
- 👀 **Group Members:** Deveepria A/P Sankaran, Nur Irdina binti Mohd Shahrir, Thulasy A/P Chandran
- 🌱 **Task description:-** We explore a keyword-based spoken language understanding system, in which the intent of the user can directly be derived from the detection of a sequence of keywords in the query. We focus on the keyword spotting method and edge impulse which is the leading development platform for machine learning on edge devices and free for developers. Edge impulse is used to perform audio data classification. In this stage 3 we are working on connection of chip(sound sensor) to ADC interface and display the reading of the sound sensor through serial communication on putty.exe. An analog-to-digital converter(ADC) converts an analog voltage to a digital value that a microcontroller can use. The code below is the part of the main.c file that used to interface sound sensor with the ADC: 

 while (1)
  {
	  	  HAL_ADC_Start(&hadc1); //start ADC conversion 
	  	  HAL_ADC_PollForConversion(&hadc1, HAL_MAX_DELAY); //Poll ADC1 with timeout 1ms
	  	  sound = HAL_ADC_GetValue(&hadc1); //Read ADC conversion result
	  	  sprintf(noise, "sound intensity : %hu\r\n",sound); //convert to string and print
	  	  HAL_UART_Transmit(&huart2, (uint8_t*)noise, strlen(noise), HAL_MAX_DELAY); //transmit the data
	  	  HAL_Delay(500); //pretend we have to do something else for a while
   }

The output "sound intensity" interface with ADC that read by the sound sensor will be displaying in the putty.exe through serial communication.



- 💞️ **Youtube:** https://www.youtube.com/watch?v=WrsuUHKdZDg
- 📫 **References:** Lecture Note, Chapter 10: Serial Interfacing https://www.hackster.io/ashish205/stm32f0-push-button-to-switch-on-led-bc9958 https://www.engineersgarage.com/insight-how-dip-switch-works/ https://www.youtube.com/watch?v=JZsC34jfbEg https://microcontrollerslab.com/push-button-control-leds-stm32f4-discovery-board-digital-input-pins-hal-driver/

# stm32-

LEDS:-

# stm32-

LED Glowing using HAL_GPIO_WritePin

LED Toggleing using HAL_GPIO_WritePin

LED Toggleing using HAL_GPIO_WritePin

LEDS glowing and toggleing with pushbutton

---------------------------------------------------------------------------------------------------------------


1.LED12 glow with HAL_GPIO_WritePin

2.LED13 glow with HAL_GPIO_WritePin

3.LED14 glow with HAL_GPIO_WritePin

4.LED14 glow with HAL_GPIO_WritePin

5.LED12 toggle with HAL_GPIO_WritePin

6.LED13 toggle with HAL_GPIO_WritePin

7.LED14 toggle with HAL_GPIO_WritePin

8.LED15 toggle with HAL_GPIO_WritePin

9.LED12 toggle with HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_12);

10.LED13 toggle with HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_13);

11.LED14 toggle with HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_14);

12.LED15 toggle with HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_15);

13.toggle all leds with round and delay

14.Push button and led on/off

push button is on then led is on

push button is off then led is off

15.when push button is on then all leds on else  leds off

16.when push button is on then  all leds off else off on

17.When push button is high then toggle leds

18.when push button is low the toggle all leds 


Sample:-


   GPIO_PinState myPushButton;
  /* Infinite loop u*/
  /* USER CODE BEGIN WHILE */
  while (1)
  {
    /* USER CODE END WHILE */
    MX_USB_HOST_Process();
    myPushButton=HAL_GPIO_ReadPin(GPIOA,GPIO_PIN_0);
    if(myPushButton==1){
    	HAL_Delay(1000);
    	HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_12);
    	HAL_Delay(1000);
    	HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_13);
    	HAL_Delay(1000);
    	HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_14);
    	HAL_Delay(1000);
    	HAL_GPIO_TogglePin(GPIOD,GPIO_PIN_15);
    	HAL_Delay(100);
    }



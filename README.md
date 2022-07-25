# stm32-

1.LED12 ON and Off with Delay








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
    	HAL_Delay(1000);
    }



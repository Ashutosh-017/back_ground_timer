I am using stm32f103c8t6 blue pill microcontroller and stm32cubeIDE. I am sharing my main.c file In this project I have created a non blocking timer.
Timer-2 and HAL libary is used in this project. 
Functioning is as follows 
The timer is hiting callback function on every 1us then in "HAL_TIM_PeriodElapsedCallback" function there is "timer_counter" variable which is globaly declared.
So when ever controller hit callback function I am increaing the value of "timer_counter" variable and making "timer_flag" HIGH when variable value reaches to 10. It means 10us.

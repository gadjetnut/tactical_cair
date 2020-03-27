Interrupt driven Arduino libary

 - Driven off Timer 0 (OCR0A) which triggers two class instances (servo and alarm)
 - Non blocking
 - Timer0 - used for millis(), micros(), delay() and PWM on pins 5 & 6
 - Timer1 - used for Servos, and PWM on pins 9 & 10
 - Timer2 - used by Tone and PWM on pins 11 & 13

Servo config:
sweep_angle=90;              //degrees
servo_speed=1;              //1=fastest 10=slower, 20=slower etc... the actual speed depends on the servo
delay_open_interval=3000;    //ms time interval the servo stays open
delay_closed_interval=1000;  //ms time interval the servo stays closed
servo_pin=9;                 //the pin driving the servo

Alarm config:
beep_interval=500;           //interval between alarm beeps
alarm_pin=11;                //the alarm pin

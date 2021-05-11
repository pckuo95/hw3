# hw3
mbed_HW3
this is a mbed code start with RPC.
RPC with two custom function:
1.sel_gesture: gestrue UI
2.tilt_detect: tilt angle detection

gestrue UI:
revised from lab8
LED2 to represent this mode
change angle via different gesture: ring for 30, slope for 45, wave for 60.
uLCD display will show selected angle.
push UserButton to confirm the angle, and stop this function.

tilt angle detection:
revised from lab10
LED3 to represent this mode
first initialize reference direction....
LED1 will blink for 1s 

then it will detect the angle and display via uLCD every 0.1s
LED2 to represent this status
when over threshold angle, it send message via MQTT
15 times will stop this function.

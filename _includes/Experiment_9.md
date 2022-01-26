# Experiment 9
## Temperature Sensor
### __ITEMS NEEDED:-__
* Arduino UNO
* A Breadboard
* Male to male jumper wires (x3)
* Temperature sensor
* USB cable to connect the arduino
* Serial monitor

### Circuit:







### Code:

 ```
int potPin = 0;
void setup()
{
Serial.begin(9600);
}
void loop()
{
int val;
int dat;
val=analogRead(0);
dat=(150*val)>>8;
Serial.print("Tep");
Serial.print(dat);
Serial.println("C");
delay(500);
}

```
### _Output:_
The temperature of the surroundings will be constantly be displayed on the serial monitor. In this case, we use the serial monitor on the arduino application itself. 

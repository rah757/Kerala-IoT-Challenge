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
![IMG_20220126_212532](https://user-images.githubusercontent.com/69799424/151199081-641f171d-8cc6-4cc6-abee-b9f51d0bd7ed.jpg)






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

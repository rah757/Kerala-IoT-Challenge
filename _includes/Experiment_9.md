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
![PXL_20220126_220826653](https://user-images.githubusercontent.com/69799424/151206705-7019c69f-45fc-4b1e-b8c7-eab39cf04ad6.jpg)







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
![Screenshot (157)](https://user-images.githubusercontent.com/69799424/151206824-3312fb22-7109-4e3f-8af2-aa4d23b3b770.png)

<iframe width="560" height="315" src="https://www.youtube.com/embed/yVaGxQcF6hs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


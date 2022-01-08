# Experiment 6
## RGB led
### __ITEMS NEEDED:-__
* Arduino UNO
* A Breadboard
* Male to male jumper wires (x4)
* RGB LED (x1)
* USB cable to connect the arduino
* Resistors

### Circuit Diagram:
![Screenshot (112)](https://user-images.githubusercontent.com/69799424/148663025-4d0894e6-efe9-47f9-82ec-8adf9b5748b2.png)




### Code:

 ```
void setup()
{
  pinMode(11, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(9, OUTPUT);
}

void loop()
{
  analogWrite(11, 255);
  analogWrite(10, 0);
  analogWrite(9, 0);
  delay(1000);
  analogWrite(11, 0);
  analogWrite(10, 255);
  analogWrite(9, 0);
  delay(1000);
  analogWrite(11, 0);
  analogWrite(10, 0);
  analogWrite(9, 255);
  delay(1000);
}

```
### _Output:_
LED starts glowing alternatively with the colors Red, Green and Blue.


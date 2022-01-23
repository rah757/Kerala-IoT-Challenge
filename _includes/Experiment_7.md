# Experiment 7
## LDR light sensor
### __ITEMS NEEDED:-__
* Arduino UNO
* A Breadboard
* Male to male jumper wires (x5)
* RGB LED (x1)
* USB cable to connect the arduino
* Resistors
* LDR

### Circuit Diagram:
![LDR](https://user-images.githubusercontent.com/69799424/150692479-b2d0739b-0018-4897-9d01-45d7c5eab585.png)





### Code:

 ```
void setup()
{
  pinMode(A0, INPUT);
  Serial.begin(9600);

  pinMode(10, OUTPUT);
}

void loop()
{
  Serial.println(analogRead(A0));
  if (analogRead(A0) < 400) {
    digitalWrite(10, HIGH);
  } else {
    digitalWrite(10, LOW);
  }
  delay(10);
}

```
### _Output:_
LED is off when there is light, when it is in the  dark the LED lights up.

<iframe width="560" height="315" src="https://www.youtube.com/embed/_G9TzlmD470" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

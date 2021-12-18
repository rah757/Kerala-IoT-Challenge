# Experiment 1
## Hello World LED Blinking
### __ITEMS NEEDED:-__
* Arduino UNO
* A Breadboard
* Male to male jumper wires (x2)
* LED 
* USB cable to connect the arduino
* Resistor

### Circuit Diagram:
![Screenshot (65)](https://user-images.githubusercontent.com/69799424/146643276-59ed5c0f-c990-4d72-8b04-df6b8b7b0084.png)

### Code:

 ```
 void setup()
{
  pinMode(8, OUTPUT);
}

void loop()
{
  digitalWrite(8, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(8, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
}

```
### _Here's a video on how the output is:_

<iframe width="560" height="315" src="https://www.youtube.com/embed/DE0KzMhWAOo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>




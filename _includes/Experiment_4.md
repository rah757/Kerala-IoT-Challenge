# Experiment 4
## Button Controlled LED
### __ITEMS NEEDED:-__
* Arduino UNO
* A Breadboard
* Male to male jumper wires (x5)
* LED (x1)
* USB cable to connect the arduino
* Resistors (10k ohm and 220 ohm)
* Button switch

### Circuit Diagram:
![Button controlled LED](https://user-images.githubusercontent.com/69799424/147852038-bb243f6e-2101-4631-a4f4-b30a19df83a2.png)



### Code:

 ```
void setup()
{
  pinMode(2, INPUT);
  pinMode(12, OUTPUT);
}

void loop()
{
  if (digitalRead(2) == HIGH) {
    digitalWrite(12, HIGH);
  } else {
    digitalWrite(12, LOW);
  }
  delay(10); // Delay a little bit to improve simulation performance
}

```
### _Output:_
We get an LED which lights up when the button is pressed.

<iframe width="560" height="315" src="https://www.youtube.com/embed/bcOF31Ylf1E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



# Experiment 8
## Flame Sensor
### __ITEMS NEEDED:-__
* Arduino UNO
* A Breadboard
* Male to male jumper wires (x5)
* Buzzer
* USB cable to connect the arduino
* Resistor
* Flame Sensor

### Circuit:
![IMG_20220126_195910](https://user-images.githubusercontent.com/69799424/151184319-afdd24b5-6b8f-461c-b644-d2c9380d1e95.jpg)






### Code:

 ```
int flame=0;
int Beep=9;
int val=0;
 void setup() 
{
  pinMode(Beep,OUTPUT);
 pinMode(flame,INPUT);
 Serial.begin(9600);
 } 
void loop() 
{ 
  val=analogRead(flame);
  Serial.println(val);
  if(val>=500)
  {  
   digitalWrite(Beep,HIGH); 
   }else 
   {  
     digitalWrite(Beep,LOW); 
    }
   delay(500); 
}

```
### _Output:_
When you apply flame/heat to the Flame sensor, the analog value of the input gets increased. When this goes over a certain level, the buzzer starts buzzing. 




const byte pHpin = A0;   
float Po;
void setup()
{
Serial.begin(9600);
}
void loop()
{
Po = 1023 - analogRead(pHpin);  
Po = map(Po, 0, 1023, 0, 14); 
Serial.println(Po);             
delay(1000);                  
}

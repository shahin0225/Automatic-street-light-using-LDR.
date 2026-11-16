# Automatic-street-light-using-LDR.
An automatic street lighting system that uses an LDR sensor to detect darkness and automatically switches ON the street lights at night and OFF during daytime, saving energy.
int LDR_Variables = 0; 

void setup() 
{ 
} 
pinMode(A0, INPUT); 
Serial.begin(9600); 
pinMode(10, OUTPUT); 
pinMode(0, OUTPUT); 
void loop() 
{ 
} 
LDR_Variables = analogRead(A0); 
Serial.println(LDR_Variables); 
if (LDR_Variables > 500) { 
digitalWrite(10, HIGH); 
} else { 
digitalWrite(0, LOW); 
} 
delay(10); // Delay a little bit to improve simulation performance

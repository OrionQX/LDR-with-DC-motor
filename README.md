# LDR-with-DC-motor

Fotodiyotlu DC Motor

int LDR = A2; 
int motorPin1 = 9; 
int motorPin2 = 10; 

void setup() {
   pinMode(9,OUTPUT);
   pinMode(10,OUTPUT);
   Serial.begin(9600);
}

void loop() {
  int light = analogRead(A2);
  Serial.println(light);
  if(light > 600){
    digitalWrite(9,LOW);
    }
  else if (light < 600){
  digitalWrite(9,HIGH);    
  }
}

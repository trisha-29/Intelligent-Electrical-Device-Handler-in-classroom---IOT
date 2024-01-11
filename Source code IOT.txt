void setup() {
 Serial.begin(9600);
 pinMode(8,INPUT);
 pinMode(9,OUTPUT);
  pinMode(13,OUTPUT);
}

void loop() {
 int data = digitalRead(8);
 Serial.println(data);

 if(data == 0)
 {
  digitalWrite(9,HIGH);
  digitalWrite(13,HIGH);
 }
 else
 {
  digitalWrite(9,LOW);
  digitalWrite(13,LOW);
 }
 delay(1000);
}  


  

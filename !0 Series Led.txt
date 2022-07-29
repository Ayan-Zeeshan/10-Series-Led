int PM = A5;
int Led = 2;
int Led2 = 3;
int Led3 = 4;
int Led4 = 5;
int Led5 = 6;
int Led6 = 7;
int value = 0;
int Led7 = 8;
int Led8 = 9;
int Led9 = 10;
int Led10 = 11;

void setup(){
pinMode(PM, INPUT);
  pinMode(Led, OUTPUT);
  pinMode(Led2, OUTPUT);
  pinMode(Led3, OUTPUT);
  pinMode(Led4, OUTPUT);
  pinMode(Led5, OUTPUT);
  pinMode(Led6, OUTPUT);
  pinMode(Led7, OUTPUT);
  pinMode(Led8, OUTPUT);
  pinMode(Led9, OUTPUT);
  pinMode(Led10, OUTPUT);
  Serial.begin(9600);
}

void loop(){
value = analogRead(PM);
  Serial.println(value);
  int brightness = map(value,  0 , 1023 , 0, 255);
  analogWrite(Led, brightness);
  delay(200);
  analogWrite(Led2, brightness);
  delay(200);
  analogWrite(Led3, brightness);
  delay(200); 
  analogWrite(Led4, brightness);
  delay(200);  
  analogWrite(Led5, brightness);
  delay(200);  
  analogWrite(Led6, brightness);
  delay(200);  
  analogWrite(Led7, brightness);
  delay(200);  
  analogWrite(Led8, brightness);
  delay(200);  
  analogWrite(Led9, brightness);
  delay(200);  
  analogWrite(Led10, brightness);
}

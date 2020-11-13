
int ENA=5;<br/>
int ENB=6;<br/>
int IN1=7;<br/>
int IN2=8;<br/>
int IN3=9;<br/>
int IN4=11;<br/>

void setup() {<br/>
  // put your setup code here, to run once:<br/>
pinMode(ENA, OUTPUT);<br/>
pinMode(ENB, OUTPUT);<br/>
pinMode(IN1, OUTPUT);<br/>
pinMode(IN2, OUTPUT);<br/>
pinMode(IN3, OUTPUT);<br/>
pinMode(IN4, OUTPUT);<br/>
digitalWrite(ENA, HIGH);<br/>
digitalWrite(ENB, HIGH);<br/>

Forward();<br/>
Left_Pivot();<br/>
Forward();<br/>
Left_Pivot();<br/>
Forward();<br/>
Left_Pivot();<br/>
Forward();<br/>
Forward();<br/>
Right_Pivot();<br/>
Forward();<br/>
Right_Pivot();<br/>
Forward();<br/>
Right_Pivot();<br/>
Forward();<br/>
}<br/>
void loop() {<br/>
  // put your main code here, to run repeatedly:<br/>
void Wait() {<br/>
  delay(375);<br/>
}<br/>
void Stop() {<br/>
  digitalWrite(IN1, LOW);<br/>
  digitalWrite(IN2, LOW);<br/>
  digitalWrite(IN3, LOW);<br/>
  digitalWrite(IN4, LOW);<br/>
  delay(375);<br/>
}<br/>
void Left_Pivot() {<br/>
  digitalWrite(IN1, LOW);<br/>
  digitalWrite(IN2, HIGH);<br/>
  digitalWrite(IN3, LOW);<br/>
  digitalWrite(IN4, HIGH);<br/>
  delay(375);<br/>
}<br/>
void Right_Pivot() {<br/>
  digitalWrite(IN1, HIGH);<br/>
  digitalWrite(IN2, LOW);<br/>
  digitalWrite(IN3, HIGH);<br/>
  digitalWrite(IN4, LOW);<br/>
  delay(375);<br/>
}<br/>
void Forward() {<br/>
  digitalWrite(IN1, HIGH);<br/>
  digitalWrite(IN2, LOW);<br/>
  digitalWrite(IN3, LOW);<br/>
  digitalWrite(IN4, HIGH);<br/>
  delay(1500);<br/>
}<br/>
void Back() {<br/>
  digitalWrite(IN1, LOW);<br/>
  digitalWrite(IN2, HIGH);<br/>
  digitalWrite(IN3, HIGH);<br/>
  digitalWrite(IN4, LOW);<br/>
  delay(1500);<br/>
}<br/>
void Left_Wide() {<br/>
  digitalWrite(IN1, LOW);<br/>
  digitalWrite(IN2, LOW);<br/>
  digitalWrite(IN3, LOW);<br/>
  digitalWrite(IN4, HIGH);<br/>
  delay(375);<br/>
}<br/>
void Right_Wide() {<br/>
  digitalWrite(IN1, LOW);<br/>
  digitalWrite(IN2, HIGH);<br/>
  digitalWrite(IN3, LOW);<br/>
  digitalWrite(IN4, LOW);<br/>
  delay(375);<br/>
}<br/>


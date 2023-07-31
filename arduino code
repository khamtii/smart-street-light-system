const int led1 = 3;
const int led2 = 5;
const int led3 = 6;
int ldr = A0;
const int ir1 = 11;
const int ir2 = 12;
const int ir3 = 13;
int a, b, c;
int ldrStatus;
void setup() {
  // put your setup code here, to run once:
  Serial.begin (9600);

  pinMode (led1, OUTPUT);
  pinMode (led2, OUTPUT);
  pinMode (led3, OUTPUT);

  pinMode (ldr, INPUT);
  pinMode (ir1, INPUT);
  pinMode (ir2, INPUT);
  pinMode (ir3, INPUT);
}

void loop() {

  // put your main code here, to run repeatedly:
  int ldrStatus = analogRead (ldr);

  a = digitalRead(ir1);
  b = digitalRead(ir2);
  c = digitalRead(ir3);

  Serial.print(a);
  Serial.print(b);
  Serial.print(c);
  Serial.print("...");
  Serial.println(ldrStatus);
  delay(200);
  //evening/night dim light
  if (ldrStatus <= 90 ) {
    analogWrite (led1, 230);
    analogWrite (led2, 230);
    analogWrite (led3, 230);
  }
  //night and ir1 senses
    if (digitalRead(ir1) == 0){
    analogWrite (led1, 10);
    delay(500);
    //analogWrite (led1, 10);
    }
 
   //night and ir2 senses
    if (digitalRead(ir2) == 0){
    analogWrite (led2, 10);
    delay(500);
    //analogWrite (led2, 0);
    }
    //night and ir3 senses
    if (digitalRead(ir3) == 0){
    analogWrite (led3, 10);
     delay(500);
    //analogWrite (led3, 70);
    }

  if (ldrStatus > 80) {
    analogWrite (led1, 255);
    analogWrite (led2, 255);
    analogWrite (led3, 255);
  }
  

}

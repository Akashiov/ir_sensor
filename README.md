# ir_sensor
// ir sensor connection with arduino code 
void setup() {
 pinMode(A0,INPUT);
 pinMode(3,OUTPUT);
 Serial.begin(9600);
  // put your setup code here, to run once:

}

void loop() {
 int a=analogRead(A0);
 Serial.println(a);
 

if(a<30){
  digitalWrite(3,1);
}
  else{
  digitalWrite(3,0);
  }

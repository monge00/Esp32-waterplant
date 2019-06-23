# Esp32-waterplant
This code will automatically dispose water in my home plants

Version #1
.No sensors connected
.Active relay periodically for certain time to turn on a water pump (20 lts gallon).

const int Relay = 3; //define digital pin 3 as relay output
void setup () {
// inicia programa
pinMode (Relay, OUTPUT); //configure the Relay pin as an Output

}

void loop () {
// repete o que for necessária para a automação
digitalWrite(Relay,HIGH); //Turn on the pump for 10 seconds
delay(10000);
digitalWrite(Relay,LOW); //Turn off the pump for 4 days
delay(5760000);

}

/*
   contact: ajiaryad@gmail.com
*/
#include <L298N.h>
#define ENA 6
#define IN1 8
#define IN2 7
#define ENB 11
#define IN3 9
#define IN4 10
int S1, S2, S3, S4, S5, S6 , S7, S8;
int SKn = 13;
int SKr = 12;


L298N motorkiri(ENA, IN1, IN2);
L298N motorkanan(ENB, IN3, IN4);

void setup() {
  Serial.begin(9600);
  pinMode(SKn, INPUT_PULLUP);
  pinMode(SKr, INPUT_PULLUP);
  delay(2000);


}

void bacaSensor() {
  S8 = digitalRead(SKn);
  S1 = digitalRead(SKr);
  int sensor1 = analogRead(A5);
  int sensor2 = analogRead(A4);
  int sensor3 = analogRead(A3);
  int sensor4 = analogRead(A2);
  int sensor5 = analogRead(A1);
  int sensor6 = analogRead(A0);

  if (sensor1 >= 500) {
    S2 = 1 ;
  }
  else {
    S2 = 0 ;
  }

  if (sensor2 >= 500) {
    S3 = 1 ;
  }
  else {
    S3 = 0 ;
  }

  if (sensor3 >= 500) {
    S4 = 1 ;
  }
  else {
    S4 = 0 ;
  }

  if (sensor4 >= 500) {
    S5 = 1 ;
  }
  else {
    S5 = 0 ;
  }

  if (sensor5 >= 500) {
    S6 = 1 ;
  }
  else {
    S6 = 0 ;
  }

  if (sensor6 >= 500) {
    S7 = 1 ;
  }
  else {
    S7 = 0 ;
  }

  Serial.print(S1);
  Serial.print(S2);
  Serial.print(S3);
  Serial.print(S4);
  Serial.print(S5);
  Serial.print(S6);
  Serial.print(S7);
  Serial.println(S8);
  delay(1);

}

void loop() {
  bacaSensor();

  if (S1 == 1 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(245);
    motorkanan.forward();
    motorkiri.setSpeed(55);
    motorkiri.backward();
  }
  else if (S1 == 1 && S2 == 1 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(245);
    motorkanan.forward();
    motorkiri.setSpeed(0);
    motorkiri.backward();
  }
  else if (S1 == 0 && S2 == 1 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(220);
    motorkanan.forward();
    motorkiri.setSpeed(50);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 1 && S3 == 1 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(190);
    motorkanan.forward();
    motorkiri.setSpeed(30);
    motorkiri.backward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 1 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(180);
    motorkanan.forward();
    motorkiri.setSpeed(50);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 1 && S4 == 1 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(150);
    motorkanan.forward();
    motorkiri.setSpeed(30);
    motorkiri.backward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 1 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(120);
    motorkanan.forward();
    motorkiri.setSpeed(30);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 1 && S5 == 1 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(40);
    motorkanan.forward();
    motorkiri.setSpeed(50);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 1 && S6 == 0 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(20);
    motorkanan.forward();
    motorkiri.setSpeed(130);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 1 && S6 == 1 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(20);
    motorkanan.backward();
    motorkiri.setSpeed(160);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 1 && S7 == 0 && S8 == 0) {
    motorkanan.setSpeed(40);
    motorkanan.forward();
    motorkiri.setSpeed(190);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 1 && S7 == 1 && S8 == 0) {
    motorkanan.setSpeed(40);
    motorkanan.forward();
    motorkiri.setSpeed(200);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 1 && S8 == 0) {
    motorkanan.setSpeed(40);
    motorkanan.forward();
    motorkiri.setSpeed(230);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 1 && S8 == 1) {
    motorkanan.setSpeed(0);
    motorkanan.backward();
    motorkiri.setSpeed(255);
    motorkiri.forward();
  }
  else if (S1 == 0 && S2 == 0 && S3 == 0 && S4 == 0 && S5 == 0 && S6 == 0 && S7 == 0 && S8 == 1) {
    motorkanan.setSpeed(45);
    motorkanan.backward();
    motorkiri.setSpeed(255);
    motorkiri.forward();

  }
}

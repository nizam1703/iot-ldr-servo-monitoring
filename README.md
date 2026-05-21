# ESP8266 LDR Servo Blynk

Projek ini merupakan sistem IoT sederhana berbasis **ESP8266** yang menggunakan sensor **LDR** untuk membaca kondisi cahaya. Hasil pembacaan cahaya digunakan untuk menggerakkan **servo** secara otomatis. Data nilai LDR dan sudut servo juga dikirim ke dashboard **Blynk** agar dapat dipantau secara real-time.

## Deskripsi Projek

Sistem ini bekerja dengan cara membaca nilai cahaya dari sensor LDR. Jika nilai LDR berada di bawah ambang batas, maka kondisi dianggap gelap dan servo akan bergerak ke posisi tertutup. Jika nilai LDR lebih dari atau sama dengan ambang batas, maka kondisi dianggap terang dan servo akan bergerak ke posisi terbuka.

Projek ini dapat digunakan sebagai contoh sistem otomatisasi berbasis cahaya, seperti tirai otomatis, penutup otomatis, atau simulasi sistem monitoring cahaya berbasis IoT.

## Komponen yang Digunakan

- ESP8266
- Sensor LDR
- Servo motor
- Resistor
- Kabel jumper
- Breadboard
- Platform Blynk
- Wokwi sebagai simulasi

## Library yang Digunakan

```cpp
#include <ESP8266WiFi.h>
#include <BlynkSimpleEsp8266.h>
#include <Servo.h>

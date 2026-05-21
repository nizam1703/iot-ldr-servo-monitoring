# ESP32 LDR Servo Blynk

Projek ini merupakan sistem IoT sederhana berbasis **ESP32** yang menggunakan sensor **LDR** untuk mendeteksi kondisi cahaya dan menggerakkan **servo** secara otomatis. Data nilai sensor LDR dan sudut servo dikirimkan ke dashboard **Blynk** agar dapat dipantau secara real-time.

## Deskripsi Projek

Sistem ini bekerja dengan cara membaca nilai cahaya dari sensor LDR. Jika nilai cahaya berada di bawah ambang batas, maka kondisi dianggap gelap dan servo akan bergerak ke posisi tertutup. Jika nilai cahaya melewati ambang batas, maka kondisi dianggap terang dan servo akan bergerak ke posisi terbuka.

Projek ini dapat digunakan sebagai contoh sederhana untuk sistem otomatisasi berbasis cahaya, seperti tirai otomatis, penutup otomatis, atau sistem monitoring cahaya berbasis IoT.

## Komponen yang Digunakan

- ESP32
- Sensor LDR
- Servo motor
- Resistor
- Kabel jumper
- Breadboard
- Platform Blynk
- Wokwi sebagai simulasi

## Library yang Digunakan

```cpp
#include <WiFi.h>
#include <BlynkSimpleEsp32.h>
#include <ESP32Servo.h>

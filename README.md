# Arduino

*Kit elektronik atau papan rangkaian elektronik open source yang di dalamnya terdapat komponen utama yaitu sebuah chip mikrokontroler dengan jenis AVR dari perusahaan Atmel*. 

## Fungsi Arduino
Software dan hardware Arduino dirancang dengan mudah digunakan untuk seniman, perancang, penggemar, peretas, pemula, dan siapa pun yang tertarik untuk membuat objek atau lingkungan interaktif. Arduino dapat berinteraksi dengan tombol, LED, motor, speaker, unit GPS, kamera, internet, dan bahkan ponsel pintar atau TV Anda! Fleksibilitas ini dikombinasikan dengan fakta bahwa software Arduino dapat didownload secara gratis, harga boardnya atau papan hardware cukup murah, dan Arduino cukup mudah dipelajari.

## Komponen Dasar yang Dibutuhkan
- Arduino
- Aplikasi Arduino
- Breadboard
- Jumper Cable
- USB Cable
- Komponen sensor yang anda inginkan

## Contoh Rangkaian Arduino
### Gambar Rangkaian
![](https://github.com/ncclaboratory18/Camin2021/blob/arduino/Custom_Mini-Piano_by_IvanAR_bisa_main_bluebird.png)

### Source Code Rangakian
```C
/*
  Keyboard

  Plays a pitch that changes based on a changing
  input circuit:
  * 3 pushbuttons from +5V to analog in 0 through
  3
  * 3 10K resistors from analog in 0 through 3 to
  ground
  * 8-ohm speaker on digital pin 8
*/

int pos = 0;

void setup()
{
  pinMode(A0, INPUT);
  pinMode(8, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(A1, INPUT);
  pinMode(A2, INPUT);
  pinMode(A3, INPUT);
  pinMode(A4, INPUT);
  pinMode(A5, INPUT);
  pinMode(2, INPUT);
  pinMode(3, INPUT);
  pinMode(4, INPUT);
  pinMode(5, INPUT);

}

void loop()
{
  if (digitalRead(A0) == HIGH) {
    tone(8, 256, 100); 
  } //play tone at 256hz to output pin 8 with duration 100
  if (digitalRead(A1) == HIGH) {
    tone(8, 285, 100); 
  }
  if (digitalRead(A2) == HIGH) {
    tone(8, 320, 100); 
  }
  if (digitalRead(A3) == HIGH) {
    tone(8, 341, 100); 
  }
  if (digitalRead(A4) == HIGH) {
    tone(8, 384, 100); 
  }
  if (digitalRead(A5) == HIGH) {
    tone(8, 427, 100); 
  }
  if (digitalRead(2) == HIGH) {
    tone(8, 480, 100); 
  }
  if (digitalRead(3) == HIGH) {
    tone(8, 512, 100); 
  }
  if (digitalRead(4) == HIGH) {
    tone(9, 570, 100); 
  }
  if (digitalRead(5) == HIGH) {
    tone(9, 640, 100); 
  }
  delay(10); // Delay a little bit to improve simulation performance
}
```

### Link Tutorial dan Referensi Belajar
- https://www.tinkercad.com/
- https://create.arduino.cc/projecthub
- https://digitalapik.blogspot.com/2019/02/mengenal-pin-pin-pada-arduino.html

## Penugasan Arduino
- Membuat suatu rangkaian yang menggunakan beberapa modul (minimal 2)
- Rangkaian yang dibuat memiliki manfaat
- Setiap individu rangkaiannya berbeda-beda

### Penilaian Arduino
- Minimal jumlah modul yang digunakan
- Kreativitas ide yang digunakan
- Pengimplementasian ide
- Keberhasilan ide
- Penyampaian ide

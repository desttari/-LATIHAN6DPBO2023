# LATIHAN7DPBO2023
Latihan 7 Synchronization

## Janji
Saya Destira Lestari Saraswati NIM 2100506 mengerjakan soal Latihan 6 dalam mata kuliah Desain Pemrograman Berorientasi Objek untuk keberkahanNya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin.

# Synchronization Game

Synchronization Game adalah sebuah game sederhana yang dibangun dengan menggunakan Java dan mengimplementasikan konsep pemrograman multithreading dan sinkronisasi. Game ini mencakup beberapa kelas dan antarmuka yang bekerja sama untuk mengatur objek game dan memastikan pemrosesan yang lancar dan sinkronisasi antara objek.

## Struktur Kode

Proyek ini terdiri dari 8 file Java yang mencakup kelas dan antarmuka berikut:

### 1. Display.java
Kelas `Display` digunakan untuk mengatur tampilan game, seperti membuat dan mengatur ukuran jendela game.

### 2. Controller.java
Kelas `Controller` mengelola input keyboard dari pemain. Ini digunakan untuk mengendalikan gerakan karakter pemain.

### 3. Game.java
Kelas `Game` adalah kelas utama yang mengelola game, termasuk menjalankan game, menggambar objek di layar, dan memastikan sinkronisasi antara objek game.

### 4. GameInterface.java
Antarmuka `GameInterface` mendefinisikan metode yang diperlukan untuk kelas yang akan menggambarkan dan memperbarui objek game.

### 5. GameObject.java
Kelas `GameObject` adalah kelas dasar untuk semua objek game. Kelas ini menyediakan atribut umum dan metode yang diperlukan oleh semua objek game.

### 6. Handler.java
Kelas `Handler` digunakan untuk mengelola objek game. Kelas ini menyimpan objek game dalam ArrayList dan menyediakan metode untuk menambah, mengakses, dan menghapus objek game.

### 7. Player.java
Kelas `Player` merupakan turunan dari kelas `GameObject` dan merepresentasikan karakter pemain dalam game. Kelas ini mengatur bentuk, posisi, dan gerakan karakter pemain.

### 8. Synchronization.java
Kelas `Synchronization` berisi metode `main` yang digunakan untuk menjalankan game.



## Batasan Program

1. Program ini hanya mendukung gerakan karakter pemain. Tidak ada objek interaktif atau musuh lain dalam game ini.

2. Hanya terdapat Score
  - Score dihitung jika:
    - Pemain menekan tombol W atau A atau S atau D atau Arrow-Up atau Arrow-Down atau Arrow-left atau Arrow-Right
  - Score tidak dihitung jika:
    - Pemain menekan tombol di atas secara berurutan, misalkan:
      - W W A S D Score akan dihitung menjadi 4.
      - W Arrow-Up A A S D Score akan dihitung menjadi 4.

## Screenshots

![Alt text](/relative/path/to/img.jpg?raw=true "Optional Title")
![Alt text](/relative/path/to/img.jpg?raw=true "Optional Title")
*Saat ini belum ada screenshot yang tersedia.*

## Kompatibilitas

Game ini kompatibel dengan sistem operasi yang mendukung Java 8 atau lebih baru, seperti Windows, macOS, dan Linux.

## Diagram UML

![Alt text](/relative/path/to/img.jpg?raw=true "Optional Title")
*Saat ini belum ada Diagram UML yang tersedia.*

## Kelas, Atribut, dan Metode

### Kelas

1. Display
2. Controller
3. Game
4. GameInterface
5. GameObject
6. Handler
7. Player
8. Synchronization

### Atribut

- Display: `width`, `height`, `title`, `frame`, `canvas`
- Controller: `handler`, `player`
- Game: `width`, `height`, `handler`, `player`, `controller`, `thread`, `running`
- GameObject: `x`, `y`, `width`, `height`, `velX`, `velY`, `type`
- Handler: `object`, `rand`
- Player: Inherits attributes from GameObject

### Metode

- Display: `createDisplay()`
- Controller: `keyPressed(KeyEvent)`, `keyReleased(KeyEvent)`
- Game: `run()`, `start()`, `stop()`, `render(Graphics)`, `loop()`, `clamp(int, int, int)`
- GameInterface: `render(Graphics)`, `loop()`
- GameObject: Various getter and setter methods, `render(Graphics)`, `loop()`
- Handler: `add(GameObject)`, `get(int)`, `count()`, `remove(int)`, `remove(GameObject)`, `render(Graphics)`, `loop()`
- Player: `render(Graphics)`, `loop()`

## Cara Menjalankan

Untuk menjalankan game ini, Anda perlu mengkompilasi dan menjalankan kelas `Synchronization`. Pastikan Anda memiliki semua file di atas dalam paket yang sama dan JDK yang sesuai terinstal.


1. Pastikan Anda memiliki Java Development Kit (JDK) versi 8 atau lebih baru diinstal pada sistem Anda.
2. Buka terminal atau Command Prompt dan navigasikan ke direktori di mana file Java berada.
3. Kompilasi semua file Java dengan menjalankan perintah: `javac synchronization/*.java`
4. Jalankan kelas utama `Synchronization` dengan perintah: `java synchronization.Synchronization`









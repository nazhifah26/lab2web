1.
![image](https://github.com/user-attachments/assets/464a52b5-b7e9-4c86-9da0-20289a5e8ecf)

2. h1 untuk gaya ke semua judul utama dihalaman.
    Intro h1 untuk menargetkan hanya judul utama yang relevan dalam 
    konteks tertentu.
3. Ketika ada deklarasi CSS secara eksternal, ditambah dengan CSS eksternal dan inline pada elemen yang sama, urutan prioritas yang berlaku dalam CSS menentukan gaya mana yang akan ditampilkan di browser. Dalam hal ini, inline CSS memiliki prioritas tertinggi, diikuti oleh CSS internal, dan terakhir CSS eksternal.

Urutan Prioritas CSS
Inline CSS: Gaya yang diterapkan langsung pada elemen HTML menggunakan atribut style. Ini memiliki prioritas tertinggi dan akan mengoverride gaya lainnya.
Internal CSS: Gaya yang didefinisikan dalam tag <style> di bagian <head> dari dokumen HTML. Ini memiliki prioritas lebih rendah dibandingkan inline CSS.
External CSS: Gaya yang didefinisikan dalam file CSS terpisah dan dihubungkan ke dokumen HTML menggunakan tag <link>. Ini memiliki prioritas terendah.

Berikut adalah contoh untuk menjelaskan bagaimana ini bekerja:
xml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="styles.css"> <!-- External CSS -->
    <style>
        p {
            color: red; /* Internal CSS */
        }
    </style>
    <title>Contoh Prioritas CSS</title>
</head>
<body>
    <p style="color: blue;">Ini adalah paragraf dengan inline CSS.</p>
</body>
</html>

Ketika menggunakan berbagai jenis deklarasi CSS, penting untuk memahami urutan prioritasnya. Inline CSS akan selalu menang atas internal dan external CSS, sehingga jika Anda ingin memastikan bahwa gaya tertentu diterapkan pada elemen tertentu, penggunaan inline CSS adalah cara yang efektif meskipun tidak selalu disarankan untuk penggunaan luas karena dapat membuat kode menjadi tidak teratur dan sulit dikelola.

4. Ketika sebuah elemen HTML memiliki ID dan class, urutan prioritas dalam CSS menentukan gaya mana yang akan diterapkan di browser. Dalam hal ini, ID selector memiliki prioritas lebih tinggi dibandingkan dengan class selector.

Urutan Prioritas CSS
Inline Styles: Gaya yang diterapkan langsung pada elemen menggunakan atribut style.
ID Selector: Gaya yang didefinisikan dengan menggunakan ID, ditulis dengan simbol #.
Class Selector: Gaya yang didefinisikan dengan menggunakan class, ditulis dengan simbol .

Berikut adalah contoh untuk menjelaskan bagaimana prioritas ini berfungsi:
xml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        #myElement {
            color: red; /* ID Selector */
        }
        .myClass {
            color: blue; /* Class Selector */
        }
    </style>
    <title>Contoh Prioritas CSS</title>
</head>
<body>
    <p id="myElement" class="myClass">Ini adalah teks contoh.</p>
</body>
</html>

Ketika menggunakan ID dan class pada elemen yang sama, gaya dari ID selector akan selalu diterapkan jika ada konflik, kecuali jika ada inline styles yang diterapkan pada elemen tersebut. Ini menunjukkan pentingnya memahami urutan prioritas dalam CSS untuk mengontrol tampilan elemen di halaman web.


pertama kita akan membuat judul dan paragraf.

![image](https://github.com/user-attachments/assets/fb7d66d5-829b-495c-b4a5-e6bc956aa7ba)

kedua mengganti warna judul dan tata letak.

![image](https://github.com/user-attachments/assets/a57867c4-105d-48a1-833d-735b2209f8be)

ketiga mengganti warna isi paragraf

![image](https://github.com/user-attachments/assets/5bf30e7a-4015-4cd1-a7c9-02d7c94e6469)

keempat memberi warna dan gaya pada menu

![image](https://github.com/user-attachments/assets/7cfe7c92-dddc-40d8-a0bb-73b59a6863d9)

kelima memberi warna dan gaya pada paragraf dan tombol selengkapnya.

![image](https://github.com/user-attachments/assets/c81cd849-0ac7-4e2f-8058-8450bcba6a2e)


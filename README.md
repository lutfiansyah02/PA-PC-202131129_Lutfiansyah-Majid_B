UAS Pengolahan Citra B
Lutfiansyah Majid
202131129

Keterangan dari UAS Pengolahan Citra bagian A (memfoto plat nomor)

Pertama memanggil fungsi fungsi yang akan digunakan
yaitu :
    1. Imutils
    2. Opencv
    3. Numpy
    4. Matplotlib

Langkah :
- Membaca foto dengan menggunakan cv2.imRead
- Lalu mengubah citra dari RGB ke Grayscale
- Menggunakan bilateral filter guna mengurangi noise pada citra
- Menggunakan cv2.drawContours untuk membantu mendeteksi tepi gambar
- Lalu menggunakan cv2.Retr_TREE untuk mengambil semua kontur dengan hirarki yang lengkap
- mengurutkan Kontur secara descending

Teori : 
Segmentasi merupakan proses memisahkan objek dari latar belakang dalam citra. Dalam konteks deteksi plat nomor, langkah pertama adalah segmentasi citra untuk memisahkan plat nomor dari latar belakangnya.
Proses untuk menemukan perbedaan intensitas piksel yang signifikan di sepanjang kontur objek ialah pengertian dari Deteksi Tepi. Dalam deteksi plat nomor, deteksi tepi dapat membantu dalam mengidentifikasi kontur plat nomor. 
Setelah plat nomor terdeteksi, maka kita melakukan pemrosesan citra biner untuk meningkatkan kualitas deteksi. Metode pengolahan biner seperti dilatasi, erosi, penghilangan noise, atau operasi morfologi lainnya dapat diterapkan untuk meningkatkan kualitas gambar biner dari plat nomor.
deteksi plat nomor adalah masalah yang kompleks dan dapat melibatkan kombinasi dari berbagai metode dan teknik untuk mencapai hasil yang akurat.
Faktor utama yang tidak dapat di hiraukan ialah pencahayaan, variasi font, rotasi, dan skalabilitas plat nomor. Faktor faktor tersebut sangat diperlukan apabila ingin melakukan scan plat nomor. Kalau tidak ada faktor tersebut, jupyter akan kesulitan untuk membaca plat yang akan digunakan.

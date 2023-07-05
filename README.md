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

- Membaca foto dengan menggunakan cv2.imRead
- Lalu mengubah citra dari RGB ke Grayscale
- Menggunakan bilateral filter guna mengurangi noise pada citra
- Menggunakan cv2.drawContours untuk membantu mendeteksi tepi gambar
- Lalu menggunakan cv2.Retr_TREE untuk mengambil semua kontur dengan hirarki yang lengkap
- mengurutkan Kontur secara descending

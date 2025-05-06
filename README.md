Tola

##

### Instal

<a href="https://update.greasyfork.org/scripts/510410/YouTube%20Live%20Chat%20Judi%20Online%20Blocker.user.js" target="_blank"><img height="44px" src="https://raw.githubusercontent.com/adamlui/chatgpt-widescreen/main/media/images/badges/greasy-fork/available-on-greasy-fork-gold-square-border-light-816x262.png" alt="Instal Melalui Usercript"></a>

##

[⚒️ Instalasi](#-instalasi) &nbsp;&nbsp;|&nbsp;&nbsp; [📜 Riwayat Perubahan](#-riwayat-perubahan) &nbsp;&nbsp;|&nbsp;&nbsp; [⭐ Star History](#-star-history)

</div>

##

## ⚒️ Instalasi

### <img style="margin: 0 2px -0.065rem 0" height=17 src="https://i.imgur.com/SATGr8j.png"> <img style="margin: 0 2px -0.035rem 1px" height=17.5 src="https://i.imgur.com/wcCg3al.png"> Userscript

1. Instal ekstensi <a href="https://www.tampermonkey.net/index.php" target="_blank">Tampermonkey</a>
2. Instal userscript <a href="https://update.greasyfork.org/scripts/510410/YouTube%20Live%20Chat%20Judi%20Online%20Blocker.user.js" target="_blank">YouTube Live Chat Judi Online Blocker</a> (akan dimuat secara otomatis di pengelola skrip pengguna)
3. Buka ekstensi Tampermonkey melalui tombol Ekstensions browser> Klik Dashboard > Klik YouTube Live Chat Judi Online Blocker > Cari baris kode 19, 20, dan 23 > Atur status filter & timestamp yang Anda inginkan

https://github.com/user-attachments/assets/54d1fadb-9b17-437f-973c-d5324972dde7

4. Buka website <a href="https://www.youtube.com/" target="_blank">www.youtube.com</a> melalui browser Desktop PC / Laptop berikut:
  * <img style="margin: 0 2px -1px 0" height=16 src="https://favicon-generator.org/favicon-generator/htdocs/favicons/2023-07-04/50a84d541c2f7c791c9c3f9faeafe352.ico.png"> `Windows`: *Chrome / Firefox / Microsoft Edge / Opera / Brave / Vivaldi*
    
  * <img style="margin: 0 2px -1px 0" height=16 src="https://favicon-generator.org/favicon-generator/htdocs/favicons/2023-07-04/afdcf7209fcd4b14fb521ee04f24e676.ico.png"> `macOS`: *Safari*
4. Pastikan anda telah login akun
5. Buka live stream yang ingin Anda tonton   
6. Lihat pada kolom live chat dan selamat mencoba 😁

<div align="center">

<br>

<b>*Contoh ketika pesan promosi yang berkaitan dengan promosi judi online (judol) DIBLOKIR</center>*</b>

![image](https://raw.githubusercontent.com/okkidwi/YouTube-Live-Chat-Judi-Online-Blocker/refs/heads/main/images/contoh-filter-pesan-diblokir.png)

<br>

<b>*Contoh ketika pesan promosi yang berkaitan dengan promosi judi online (judol) DISEMBUNYIKAN</center>*</b>

![image](https://raw.githubusercontent.com/okkidwi/YouTube-Live-Chat-Judi-Online-Blocker/refs/heads/main/images/contoh-filter-pesan-disembunyikan.png)

<br>

<b>*Contoh ketika pesan promosi yang berkaitan dengan promosi judi online (judol) NONAKTIF</center>*</b>

![image](https://raw.githubusercontent.com/okkidwi/YouTube-Live-Chat-Judi-Online-Blocker/refs/heads/main/images/contoh-filter-pesan-nonaktif.png)

</div>

## 📜 Riwayat Perubahan

### **v1.6**

<details>
<summary>TEKAN UNTUK MELIHAT</summary>

- **Perbaikan Bug**:

   - Memperbaiki bug pada fungsi flag `isMasking` yang aktif ketika tombol toggle nonaktif

</details>

### **v1.5**

<details>
<summary>TEKAN UNTUK MELIHAT</summary>

- **Peningkatan Interaksi Tombol**:
   - Mengubah nama flag `isActive` menjadi `isBlocking` agar lebih sesuai

- **Penambahan Fitur Timestamp**:
   - Menambahkan kemampuan untuk menampilkan timestamp melalui fungsi `generateTimestamp24()` pada setiap pesan di live chat dalam format 24 jam (HH:MM:SS) dan fungsi `appendTimestamp`. Fitur ini dapat diaktifkan atau dinonaktifkan melalui flag `isTimestamp`.
   - Timestamp akan ditambahkan baik pada pesan yang diblokir maupun pesan yang terlihat untuk memberikan konteks lebih baik selama live streaming.

- **Optimisasi Filter dan Tampilan**:
  - **Penggunaan `MutationObserver`** dioptimalkan untuk memantau perubahan di live chat, memastikan bahwa pesan yang baru masuk difilter secara efisien.
  - **CSS diperbarui** untuk mendukung tampilan pesan yang disembunyikan dan menampilkan pesan dengan warna serta format yang berbeda.
  
</details>

### **v1.4**

<details>
<summary>TEKAN UNTUK MELIHAT</summary>

- **Penambahan Fitur Sembunyikan Pesan**:
  - Menambahkan opsi untuk menyembunyikan pesan terkait promosi judi online tanpa memblokirnya sepenuhnya. Pesan yang terdeteksi akan diganti dengan teks "[PESAN DISEMBUNYIKAN]".
  - Pesan yang disembunyikan dapat dilihat kembali dengan mengarahkan kursor (hover) pada pesan tersebut.

- **Status Blokir dan Sembunyikan Terpisah**:
  - Menambahkan flag `isMasking` untuk mengatur status sembunyikan pesan secara terpisah dari status blokir (`isActive`).
  - Pengguna dapat memilih untuk memblokir atau hanya menyembunyikan pesan terkait promosi judi online.

- **Penyempurnaan UI Tombol Toggle**:
  - Tombol toggle kini memiliki tiga status:
    1. **🔇 PROMOSI JUDOL : NONAKTIF** - Filter tidak aktif, pesan tidak diblokir atau disembunyikan.
    2. **🔇 PROMOSI JUDOL : DIBLOKIR** - Pesan terkait promosi judi online akan diblokir.
    3. **🔇 PROMOSI JUDOL : DISEMBUNYIKAN** - Pesan terkait promosi judi online akan disembunyikan.
  - Warna tombol menyesuaikan status:
    - Merah: Filter nonaktif.
    - Hijau: Pesan diblokir.
    - Oranye: Pesan disembunyikan.

- **Perbaikan Performa dan Pengamatan Elemen Chat**:
  - Memperbaiki pemantauan elemen chat untuk mendukung lebih banyak struktur DOM YouTube yang berbeda.
  - Mengurangi penggunaan `MutationObserver` untuk meningkatkan performa.

- **Penyempurnaan CSS**:
  - Memperbaiki CSS agar pesan yang diblokir atau disembunyikan tidak mengganggu tampilan keseluruhan chat.
  - Warna teks untuk pesan yang disembunyikan diperbarui agar lebih mudah dikenali (oranye).

- **Refaktor Kode**:
  - Merapikan dan memperbaiki beberapa bagian kode untuk meningkatkan keterbacaan dan efisiensi.

</details>

### **v1.3**

<details>
<summary>TEKAN UNTUK MELIHAT</summary>

- **Pembaruan Nama dan Ikon Tombol Toggle**:
  - Nama tombol toggle diperbarui dengan menambahkan ikon emoji untuk meningkatkan visual dan kejelasan status filter.
  - **Status Aktif**: Tombol akan menampilkan teks **"🔇 JUDOL : AKTIF"** ketika filter aktif.
  - **Status Nonaktif**: Tombol akan menampilkan teks **"🔇 JUDOL : NONAKTIF"** ketika filter nonaktif.

- **Penyesuaian Posisi dan Tampilan Tombol Toggle**:
  - Posisi tombol toggle diubah sedikit ke kanan dengan koordinat `top: 5px; right: 95px;` agar lebih mudah diakses dan terlihat.
  - Border-radius tombol diperhalus menjadi `8px` untuk tampilan yang lebih modern dan menarik.

</details>

### **v1.2**

<details>
<summary>TEKAN UNTUK MELIHAT</summary>

- **Peningkatan Tipe Filter**:
  - Menggunakan tipe `regexp` untuk semua aturan filter agar lebih fleksibel dan akurat dalam mengenali berbagai variasi teks.

- **Penyempurnaan Pola Regex**:
  - Aturan filter ditingkatkan dengan pola regex yang lebih kompleks dan canggih. Kini dapat mengenali variasi teks yang lebih rumit, seperti: "m+a4+x+w+i+n", "j+a4+c+k+p+o0+t+", "w+e+d+e", serta pola yang mengandung simbol dan angka.

- **Penambahan Filter Khusus**:
  - Menambahkan filter khusus untuk emoji, tanda baca, simbol matematika, dan karakter dengan aksara diakritik, sehingga dapat menangani lebih banyak variasi konten.

- **Peningkatan Fungsi `normalizeText()`**:
  - Fungsi `normalizeText()` lebih kuat dengan penambahan penghapusan karakter non-ASCII menggunakan `replace(/[^\p{ASCII}]/gu, "")`.
  - Tetap menggunakan `replace(/[\u0300-\u036f]/g, "")` untuk menghapus aksara diakritik, sehingga menghasilkan teks yang lebih bersih untuk dibandingkan dengan aturan filter.

- **Optimalisasi Metode `filterMessages()`**:
  - Menggunakan `new RegExp` untuk mencocokkan pola teks yang lebih kompleks, sehingga lebih fleksibel terhadap variasi teks yang berbeda.

- **Fungsi `updateToggleButton()` yang Lebih Terstruktur**:
  - Memperbarui fungsi `updateToggleButton()` untuk memperbaiki tampilan dan status tombol toggle. Fungsi ini kini memiliki struktur yang lebih baik untuk memudahkan pemeliharaan dan pengembangan di masa depan.

- **Penambahan CSS yang Lebih Kompleks**:
  - Penambahan dan penyempurnaan aturan CSS untuk menangani berbagai elemen, termasuk emoji, simbol, dan karakter non-ASCII, agar tampilan lebih konsisten dan dapat diandalkan.

- **Optimalisasi `MutationObserver`**:
  - `MutationObserver` dioptimalkan untuk memproses node tambahan dengan filter yang lebih canggih, memungkinkan deteksi perubahan DOM yang lebih efisien.

- **Penambahan Filter Emoji dan Simbol**:
  - Menambahkan filter khusus untuk emoji, simbol matematika, dan aksara diakritik, fitur yang belum ada pada versi 1.1.

</details>

### **v1.1**

<details>
<summary>TEKAN UNTUK MELIHAT</summary>

- **Perbaikan Tampilan Tombol**:
  - Menambahkan gaya `border-radius` (rounded) pada tombol filter untuk tampilan yang lebih halus dan modern.

</details>

### **v1.0**

<details>
<summary>TEKAN UNTUK MELIHAT</summary>

- **Pengenalan Fitur Pemblokiran Pesan**:
  - Memblokir pesan yang mengandung kata kunci tertentu, seperti: `maxwin`, `jackpot`, `petir`, `zeus`, `kakek`, `gacor`, `wd`, `wede`, `depo`, `web`, dan `situs`, untuk mengurangi konten yang tidak diinginkan.
 
</details>

## ⭐ Star History

<div align="center">

<img src="https://api.star-history.com/svg?repos=okkidwi/YouTube-Live-Chat-Judi-Online-Blocker&type=Date" width="600" height="400" alt="Star History Chart" valign="middle">
    
</div>    

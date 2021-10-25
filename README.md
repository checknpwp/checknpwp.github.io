# Indonesian NPWP Checker
Ini adalah layanan untuk pengecekan NPWP Indonesia

### Cara penggunaan

bisa langsung akses [checknpwp.github.io](https://checknpwp.github.io).
dan memasukan npwp yang di inginkan.

untuk pengunaan api bisa mengunakan Metode GET, dan aktifkan Follow Redirect

```
curl -L https://script.google.com/macros/s/AKfycbyOJ9QVzmOoBbAMYt94OoL1yMCkW-utQ7MxlU19e__iulNKQ8Y/exec?npwp=(isi NPWP tanpa format, hanya nomor)
```

tinggal di sesuaikan..

### Arti Kode Seri NPWP
Kartu NPWP memiliki kode seri dengan 15 (lima belas) angka, yang menggunakan format seperti berikut: 99.999.999.9-999.999.

 * Dua digit pertama, (99).xxx.xxx.x-xxx.xxx menunjukkan Identitas Wajib Pajak, yaitu:

   * 01 sampai 03 adalah Wajib Pajak Badan
   *  04 dan 06 adalah Wajib Pajak Pengusaha
   *  05 adalah Wajib Pajak Karyawan
   *  07 sampai 09 adalah Wajib Pajak Orang Pribadi


 * Enam digit berikut, xx.(999.999).x-xxx.xxx menunjukkan Nomor Registrasi / Urut yang diberikan Kantor Pusat Direktorat Jenderal Pajak kepada Kantor Pelayanan Pajak (KPP).
 * Satu digit berikutnya xx.xxx.xxx.(9)-xxx.xxx berfungsi sebagai Alat Pengaman untuk menghindari terjadinya pemalsuan atau kesalahan pada NPWP.

 * Tiga digit berikutnya, xx.xx.xxx.x-(999).xxx adalah Kode KPP. Jika Misalkan kodenya adalah 001, berarti NPWP tersebut dikeluarkan di KPP Pratama Jakarta Matraman, kode 061 dikeluarkan di KPP Pratama Jakarta Pancoran dan seterusnya.

 * Tiga digit terakhir, xx.xxx.xxx.x-xxx.(999) menunjukkan Status Wajib Pajak:

Kode 000 berarti berstatus Tunggal / Pusat (biasa disebut NPWP Pusat)
00x (001,002 dst) berarti Cabang, dimana angka akhir menunjukkan urutan cabang (cabang ke-1 maka 001; cabang ke-2 maka 002; dst.).

lalu jika untuk pribadi merujuk pada PERATURAN DIREKTUR JENDERAL PAJAK
NOMOR PER - 51/PJ/2008 tentang TATA CARA PENDAFTARAN NOMOR POKOK WAJIB PAJAK BAGI ANGGOTA KELUARGA
Tiga digit terakhir merupakan kode cabang, yang dimulai dari 999 bagi anggota keluarga pertama, 998 bagi anggota keluarga kedua, dan seterusnya.
npwp yang terdaftar sebelum PER-51/PJ/2008 berlaku banyak yang mengunakan 001 untuk anggota keluarga pertama

untuk pendapat lebih baik silahkan melakukan konsultasi dengan Account Representative pada KPP dimana NPWP terdaftar.
Jika NPWP Anda hilang atau rusak, disarankan untuk segera melaporkan hal tersebut ke KPP terdekat. untuk mencetak bisa mencetak secara mandiri dengan melakukan login di [djponline.pajak.go.id](https://djponline.pajak.go.id).

Mohon Gunakan Dengan Bijak, dan jangan disalahgunakan.

Dalam hal apapun Saya Pribadi tidak bertanggung jawab atas kerugian atau kerusakan termasuk tanpa batasan, kerugian tidak langsung atau kerusakan apapun yang timbul dari atau keuntungan yang timbul dari penggunaan website ini.

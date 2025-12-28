<!-- 🌐 HEADER -->
<h1 align="center">📘 Repository Jobsheet Praktikum Pemrograman Jaringan</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/VS%20Code-0078D4?style=for-the-badge&logo=visualstudiocode&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</p>

<p align="center">
  Repository ini dibuat sebagai tempat pengumpulan seluruh <b>Jobsheet Praktikum Pemrograman Jaringan 🚀</b><br>
</p>

---

## 👤 Identitas Mahasiswa

<table>
  <tr>
    <th>Nama</th>
    <td>Ridho Hamdani Putra</td>
  </tr>
  <tr>
    <th>NIM</th>
    <td>23343052</td>
  </tr>
  <tr>
    <th>Program Studi</th>
    <td>Informatika</td>
  </tr>
  <tr>
    <th>Universitas</th>
    <td>Universitas Negeri Padang</td>
  </tr>
  <tr>
    <th>Kelas</th>
    <td>INF1.62.5010</td>
  </tr>
  <tr>
    <th>Dosen Pengampu</th>
    <td>Randi Proska Sandra, S.Pd, M.Sc</td>
  </tr>
</table>

---


## 📂 Deskripsi
Repository ini berisi kumpulan *jobsheet praktikum* yang telah dikerjakan selama mata kuliah **Pemrograman Jaringan**.  
Setiap jobsheet membahas topik berbeda yang berfokus pada konsep **komunikasi jaringan menggunakan Node.js**, mulai dari dasar hingga implementasi nyata seperti server, modul, dan API.

📌 **Struktur folder:**

---

## 🧠 Daftar Rangkuman Jobsheet
> ✨ Klik salah satu jobsheet di bawah ini untuk melihat rangkuman materi.

| 🏷️ | 📚 **Jobsheet** | 🔗 **Rangkuman** |
|:--:|:----------------|:----------------|
| ✅ | **Jobsheet 1 – Pengantar Node.js** | [📘 Lihat Rangkuman](#-jobsheet-1--pengantar-nodejs) |
| ⏳ | **Jobsheet 2 – JavaScript Essentials** | *Segera ditambahkan...* |
| ✅ | **Jobsheet 3 – Module System & Command Line Arguments** | [📘 Lihat Rangkuman](#-jobsheet-3--module-system--command-line-arguments) |
| ⏳ | **Jobsheet 4 – HTTP Request and API** | *Segera ditambahkan...* |
| ⏳ | **Jobsheet 5 – Web Server dan Express.js** | *Segera ditambahkan...* |
| ⏳ | **Jobsheet 6 – JSON HTTP Endpoints** | *Segera ditambahkan...* |
| ⏳ | **Jobsheet 7 – Version Control, Git and App Deployment** | *Segera ditambahkan...* |
| ⏳ | **Jobsheet 8 – MongoDB and No-SQL Databases** | *Segera ditambahkan...* |

---

## 💡 Jobsheet 1 – Pengantar Node.js

### 📘 Deskripsi
Jobsheet pertama membahas dasar pemrograman berbasis jaringan menggunakan **Node.js**.  
Praktikum ini mencakup:
- 🔹 Pengenalan konsep *client-server*  
- 🔹 Instalasi Node.js dan Visual Studio Code  
- 🔹 Pembuatan program sederhana “Hello World”  
- 🔹 Pemahaman model *asynchronous* dan *event-driven* pada Node.js  

Node.js berfungsi sebagai runtime JavaScript di sisi server yang mendukung efisiensi dan skalabilitas tinggi.  
Melalui praktikum ini, diperlihatkan dasar cara kerja Node.js dari perintah sederhana hingga implementasi server kecil.

---

## 💡 Jobsheet 2 – JavaScript Essentials
JobSheet 2 tidak disertai direktori tersendiri karena seluruh materi dipelajari langsung melalui platform NetAcad. Topik yang dibahas mencakup konsep dasar JavaScript, seperti penggunaan variabel, jenis tipe data, operator, percabangan dan perulangan (if, for, while), pembuatan fungsi, serta pengolahan array.

---

## 💡 Jobsheet 3 – Module System & Command Line Arguments

#### 🔹 1. Sistem Modul Node.js  
Node.js menggunakan standar **CommonJS**, di mana setiap file JavaScript dianggap sebagai satu modul yang dapat diekspor dan diimpor. Sistem modul memungkinkan pemisahan logika program menjadi bagian-bagian kecil sehingga kode lebih terstruktur, mudah dibaca, dan dapat digunakan kembali di berbagai file.

<details>
  
```js
// catatan.js
const ambilCatatan = () => 'Ini adalah catatan sederhana'
module.exports = ambilCatatan
```
<i>Mengekspor fungsi dari file catatan.js agar dapat digunakan pada file lain menggunakan require().".</i>
</details> 

#### 🔹 2. Node Package Manager (NPM)  
Node Package Manager (NPM) digunakan untuk mengelola dependensi dalam proyek Node.js, di mana seluruh package yang digunakan dicatat di dalam file package.json untuk memudahkan instalasi dan pengelolaan library eksternal.

<details>
  
```js
const validator = require('validator')
console.log(validator.isURL('https://nodejs.org'))
```
<i>Penggunaan package validator untuk memeriksa apakah sebuah string merupakan URL yang valid.".</i>
</details> 

#### 🔹 3. Command Line Arguments  
Node.js dapat menerima input dari terminal melalui command line arguments yang diakses menggunakan process.argv, sehingga aplikasi dapat dijalankan dengan berbagai perintah sesuai kebutuhan pengguna.

<details>
  
```js
const command = process.argv[2]

if (command === 'tambah') {
  console.log('Perintah tambah dijalankan')
}
```
<i>Membaca argumen ketiga dari terminal untuk menentukan perintah yang dijalankan oleh program.".</i>
</details> 

#### 🔹 4. Yargs – Argument Parsing  
Yargs adalah library yang digunakan untuk mempermudah pembuatan aplikasi Command Line Interface (CLI) dengan struktur perintah yang lebih rapi, lengkap dengan deskripsi dan handler.

<details>
  
```js
const yargs = require('yargs')

yargs.command({
  command: 'tambah',
  describe: 'Menambah catatan baru',
  handler() {
    console.log('Catatan berhasil ditambahkan')
  }
})

yargs.parse()
```
<i>Mendefinisikan perintah tambah pada aplikasi CLI menggunakan Yargs.".</i>
</details> 

#### 🔹 5. Implementasi Aplikasi “Buku Catatan”  
Seluruh konsep pada jobsheet ini diterapkan dalam aplikasi buku catatan berbasis CLI yang mampu menambah, menghapus, menampilkan, dan membaca catatan, dengan data disimpan dalam format JSON menggunakan module fs.

<details>
  
```js
[
  {
    "judul": "Catatan 1",
    "isi": "Ini adalah isi catatan pertama"
  }
]
```
<i>Format penyimpanan data catatan agar mudah dibaca dan dikelola oleh aplikasi.".</i>
</details> 

---

## 💡 Jobsheet 4 – HTTP Request and API

---

## 💡 Jobsheet 5 – Web Server dan Express.js

---

## 💡 Jobsheet 6 – JSON HTTP Endpoints

---

## 💡 Jobsheet 7 – Version Control, Git and App Deployment

---

## 💡 Jobsheet 8 – MongoDB and No-SQL Databases

---

<p align="center">⚡️──────────────────────────────────────────────⚡️</p>

<p align="center">
  Made with by <b>Ridho Hamdani Putra</b><br>
  <a href="https://github.com/RidhoHamdaniPutra" target="_blank">🌐 Kunjungi Profil GitHub</a> |
  <a href="#top">⬆️ Kembali ke Atas</a>
</p>

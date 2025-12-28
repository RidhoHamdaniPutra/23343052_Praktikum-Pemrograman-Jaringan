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
<p align="justify">
Repository ini berisi kumpulan *jobsheet praktikum* yang telah dikerjakan selama mata kuliah **Pemrograman Jaringan**.  
Setiap jobsheet membahas topik berbeda yang berfokus pada konsep **komunikasi jaringan menggunakan Node.js**, mulai dari dasar hingga implementasi nyata seperti server, modul, dan API.
</p>

---

## 🧠 Daftar Rangkuman Jobsheet
> ✨ Klik salah satu jobsheet di bawah ini untuk melihat rangkuman materi.

| 🏷️ | 📚 **Jobsheet** | 🔗 **Rangkuman** |
|:--:|:----------------|:----------------|
| ✅ | **Jobsheet 1 – Pengantar Node.js** | [📘 Lihat Rangkuman](#-jobsheet-1--pengantar-nodejs) |
| ✅ | **Jobsheet 2 – JavaScript Essentials** | [📘 Lihat Rangkuman](#-jobsheet-2--javascript-essentials) |
| ✅ | **Jobsheet 3 – Module System & Command Line Arguments** | [📘 Lihat Rangkuman](#-jobsheet-3--module-system--command-line-arguments) |
| ✅ | **Jobsheet 4 – HTTP Request and API** | [📘 Lihat Rangkuman](#-jobsheet-4--http-request-and-api) |
| ✅ | **Jobsheet 5 – Web Server dan Express.js** | [📘 Lihat Rangkuman](#-jobsheet-5--web-server-dan-expressjs) |
| ✅ | **Jobsheet 6 – JSON HTTP Endpoints** | [📘 Lihat Rangkuman](#-jobsheet-6--json-http-endpoints) |
| ✅ | **Jobsheet 7 – Version Control, Git and App Deployment** | [📘 Lihat Rangkuman](#-jobsheet-7--version-control-git-and-app-deployment) |
| ✅ | **Jobsheet 8 – MongoDB and No-SQL Databases** | [📘 Lihat Rangkuman](#-jobsheet-8--mongodb-and-no-sql-databases) |
| ✅ | **Jobsheet 9 – Socket Programming** | [📘 Lihat Rangkuman](#-jobsheet-9--socket-programming) |

---

## 💡 Jobsheet 1 – Pengantar Node.js
<p align="justify">
Jobsheet 1 membahas pengenalan dasar <strong>Node.js</strong> sebagai runtime JavaScript di sisi server yang mendukung pemrograman jaringan berbasis model <strong>client–server</strong>. Pada praktikum ini dilakukan instalasi Node.js dan Visual Studio Code, pembuatan program sederhana “Hello World”, serta pengenalan konsep <strong>asynchronous</strong> dan <strong>event-driven</strong> yang menjadi karakteristik utama Node.js. Melalui jobsheet ini, mahasiswa memahami cara kerja dasar Node.js dalam mengeksekusi perintah, menangani proses non-blocking, dan membangun aplikasi server sederhana secara efisien dan skalabel.
</p>

---

## 💡 Jobsheet 2 – JavaScript Essentials
<p align="justify">
JobSheet 2 tidak disertai direktori tersendiri karena seluruh materi dipelajari langsung melalui platform NetAcad. Topik yang dibahas mencakup konsep dasar JavaScript, seperti penggunaan variabel, jenis tipe data, operator, percabangan dan perulangan (if, for, while), pembuatan fungsi, serta pengolahan array.
</p>

---

## 💡 Jobsheet 3 – Module System & Command Line Arguments
<p align="justify">
Jobsheet 3 membahas konsep <strong>modularisasi pada Node.js</strong> menggunakan sistem modul <strong>CommonJS</strong>, pengelolaan dependensi melalui <strong>Node Package Manager (NPM)</strong>, serta pemrosesan <strong>command line arguments</strong> untuk membangun aplikasi berbasis <strong>Command Line Interface (CLI)</strong>. Pada jobsheet ini, program dikembangkan secara terstruktur dengan memisahkan kode ke dalam beberapa modul, memanfaatkan package eksternal seperti <strong>chalk</strong>, <strong>validator</strong>, dan <strong>yargs</strong>, serta mengontrol alur program melalui perintah terminal. Seluruh konsep tersebut diterapkan dalam pembuatan aplikasi <strong>buku catatan CLI</strong> yang mampu menambah, menghapus, menampilkan, dan membaca catatan dengan penyimpanan data berbasis file JSON.
</p>

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
</details> 

---

## 💡 Jobsheet 4 – HTTP Request and API
<p align="justify">
Jobsheet 4 membahas konsep dasar <strong>HTTP Request</strong> dan <strong>Application Programming Interface (API)</strong> dalam pengembangan aplikasi Node.js, khususnya pada model komunikasi client–server berbasis request–response. Pada praktikum ini dipelajari cara melakukan HTTP request ke API eksternal menggunakan package postman-request, memahami struktur data <strong>JSON</strong>, serta mengolah data hasil respons dari server. Selain itu, dilakukan integrasi API Mapbox untuk mengubah nama lokasi menjadi koordinat geografis (geocoding) dan API Weatherstack untuk menampilkan informasi cuaca berdasarkan lokasi tersebut, sehingga aplikasi mampu menampilkan data real-time secara dinamis dari layanan pihak ketiga.
</p>

<details>
  
```js
const request = require('postman-request')

const url = 'http://api.weatherstack.com/current?access_key=API_KEY&query=Padang'

request({ url: url, json: true }, (error, response) => {
  console.log(response.body.current.temperature)
})
```
</details> 

---

## 💡 Jobsheet 5 – Web Server dan Express.js
<p align="justify">
Jobsheet 5 membahas konsep <strong>web server</strong> serta penggunaan <strong>Express.js</strong> sebagai web framework di atas Node.js untuk membangun aplikasi web sisi server. Pada praktikum ini dipelajari cara membuat server HTTP sederhana, mendefinisikan routing menggunakan metode app.get, mengirimkan respons dalam bentuk <strong>HTML</strong> dan <strong>JSON</strong>, serta melayani static assets seperti file CSS, JavaScript, dan gambar. Selain itu, jobsheet ini juga memperkenalkan penggunaan templating engine Handlebars (hbs) untuk memisahkan logika aplikasi dan tampilan, pembuatan halaman dinamis, serta penanganan halaman tidak ditemukan menggunakan wildcard route (404), sehingga aplikasi web menjadi lebih terstruktur, dinamis, dan mudah dikembangkan.
</p>

<details>
  
```js
const express = require('express')
const app = express()

app.get('/', (req, res) => {
  res.send('Selamat datang di halaman utama')
})

app.listen(4000, () => {
  console.log('Server berjalan pada port 4000')
})
```
</details> 
---

## 💡 Jobsheet 6 – JSON HTTP Endpoints
<p align="justify">
Jobsheet 6 membahas konsep <strong>JSON HTTP Endpoints</strong> sebagai bagian penting dalam pengembangan aplikasi web berbasis API menggunakan <strong>Express.js</strong>. Pada jobsheet ini dipelajari bagaimana server menyediakan data dalam format <strong>JSON</strong> melalui URL tertentu, memanfaatkan query string menggunakan req.query, serta membedakan antara endpoint statis dan dinamis. Praktikum juga mencakup integrasi layanan pihak ketiga menggunakan HTTP request untuk mengambil data lokasi dan cuaca, kemudian mengembalikannya dalam bentuk JSON ke klien. Selain itu, jobsheet ini menggabungkan penggunaan API eksternal, modularisasi kode dengan utilitas terpisah, serta pemanggilan endpoint melalui fetch API di sisi klien, sehingga menghasilkan aplikasi cek cuaca yang interaktif dan dinamis.
</p>

<details>
  
```js
app.get('/infocuaca', (req, res) => {
  if (!req.query.address) {
    return res.send({ error: 'Kamu harus memasukan lokasi yang ingin dicari' })
  }

  res.send({
    prediksiCuaca: 'Cuaca Sedang Hujan',
    lokasi: 'Padang',
    address: req.query.address
  })
})
```
</details> 
---

## 💡 Jobsheet 7 – Version Control, Git and App Deployment
<p align="justify">
Jobsheet 7 membahas penerapan <strong>Version Control System</strong> menggunakan <strong>Git</strong> serta proses <strong>deployment aplikasi Node.js</strong> ke lingkungan produksi. Pada jobsheet ini dipelajari konsep dasar version control seperti repository, commit, branch, merge, dan remote repository untuk mendukung kolaborasi pengembangan aplikasi secara terstruktur dan terdokumentasi. Praktikum mencakup inisialisasi repository Git, pengelolaan perubahan kode, penggunaan .gitignore, serta sinkronisasi proyek ke GitHub menggunakan SSH key. Selain itu, jobsheet ini juga membahas proses deployment aplikasi web ke platform cloud Cyclic, termasuk konfigurasi port dinamis menggunakan environment variable, penyesuaian script pada package.json, serta memastikan aplikasi dapat diakses secara online oleh pengguna akhir.
</p>

<details>
  
```js
const port = process.env.PORT || 3000

app.listen(port, () => {
  console.log('Server berjalan pada port ' + port)
})
```
</details> 
---

## 💡 Jobsheet 8 – MongoDB and No-SQL Databases
<p align="justify">
Jobsheet 8 membahas penggunaan <strong>MongoDB</strong> sebagai <strong>NoSQL Database Server</strong> pada aplikasi Node.js untuk menyimpan dan mengelola data secara fleksibel dan terstruktur dalam format dokumen. Pada praktikum ini dipelajari konsep dasar database NoSQL, perbedaan MongoDB dengan database relasional, serta proses koneksi aplikasi Node.js ke MongoDB menggunakan <strong>MongoDB Node.js Driver</strong>. Materi juga mencakup pembuatan database dan collection, operasi CRUD (Create, Read, Update, Delete), serta pemanfaatan ObjectId sebagai identitas unik setiap dokumen. Dengan penerapan MongoDB, aplikasi menjadi lebih skalabel dan efisien dalam menangani data berbasis JSON pada sistem backend modern.
</p>

<details>
  
```js
const { MongoClient } = require('mongodb')

const url = 'mongodb://127.0.0.1:27017'
const client = new MongoClient(url)

client.connect().then(() => {
  const db = client.db('task-manager')
  console.log('Berhasil terhubung ke MongoDB')
})
```
</details> 
---

## 💡 Jobsheet 9 – Socket Programming
<p align="justify">
Jobsheet 9 membahas penerapan <strong>Socket Programming</strong> untuk membangun komunikasi <strong>real-time dua arah</strong> antara client dan server menggunakan <strong>WebSocket</strong> dengan bantuan library <strong>Socket.IO</strong> pada Node.js. Pada praktikum ini dipelajari konsep dasar socket sebagai endpoint komunikasi jaringan, perbedaan komunikasi berbasis HTTP dan WebSocket, serta mekanisme event-based communication yang memungkinkan pengiriman dan penerimaan data tanpa harus melakukan request berulang. Implementasi dilakukan melalui aplikasi ruang obrolan (chat) yang mendukung pengiriman pesan teks dan lokasi secara langsung antar pengguna dalam satu room, pengelolaan user yang bergabung dan keluar, serta penggunaan library pendukung seperti Mustache untuk template tampilan, Moment untuk format waktu, dan Qs untuk parsing parameter URL. Dengan pendekatan ini, aplikasi mampu memberikan respons cepat dan interaksi real-time yang efisien.
</p>

<details>
  
```js
io.on('connection', (socket) => {
  socket.on('kirimPesan', (pesan) => {
    io.emit('pesan', pesan)
  })
})
```
</details> 
---

<p align="center">⚡️──────────────────────────────────────────────⚡️</p>

<p align="center">
  Made with by <b>Ridho Hamdani Putra</b><br>
  <a href="https://github.com/RidhoHamdaniPutra" target="_blank">🌐 Kunjungi Profil GitHub</a> |
  <a href="#top">⬆️ Kembali ke Atas</a>
</p>

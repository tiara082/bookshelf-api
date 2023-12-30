# bookshelf-api
Ini adalah proyek tugas submission untuk kelas "Belajar Membuat Aplikasi Back-End untuk Pemula" dari Dicoding. Proyek ini adalah implementasi sederhana dari API untuk manajemen buku.

## Instruksi Submission

Berikut adalah instruksi untuk menyelesaikan submission "Bookshelf API" pada kelas "Belajar Membuat Aplikasi Back-End untuk Pemula" dari Dicoding.

### Kriteria Pengujian

Terdapat 7 kriteria utama yang harus Anda penuhi dalam membuat proyek Bookshelf API.

#### Kriteria 1: Aplikasi menggunakan port 9000

Aplikasi harus menggunakan port 9000. Jika tidak memungkinkan, dapat menggunakan port lain, namun, saat pengiriman submission, gantilah portnya menjadi 9000.

#### Kriteria 2: Aplikasi dijalankan dengan perintah npm run start

Pastikan aplikasi dapat dijalankan dengan perintah npm run start. Perhatikan penggunaan nodemon, jika digunakan selama pengembangan, masukkan nodemon ke dalam runner script terpisah.

#### Kriteria 3: API dapat menyimpan buku

API harus dapat menyimpan buku melalui route:

- **Method**: POST
- **URL**: /books
- **Body Request**:

```json
{
    "name": "string",
    "year": "number",
    "author": "string",
    "summary": "string",
    "publisher": "string",
    "pageCount": "number",
    "readPage": "number",
    "reading": "boolean"
}
```

Objek buku yang disimpan pada server harus memiliki struktur sesuai dengan contoh yang diberikan.

#### Kriteria 4: API dapat menampilkan seluruh buku

API harus dapat menampilkan seluruh buku yang disimpan melalui route:

- **Method**: GET
- **URL**: /books

#### Kriteria 5: API dapat menampilkan detail buku

API harus dapat menampilkan detail buku melalui route:

- **Method**: GET
- **URL**: /books/{bookId}

#### Kriteria 6: API dapat mengubah data buku

API harus dapat mengubah data buku berdasarkan id melalui route:

- **Method**: PUT
- **URL**: /books/{bookId}
- **Body Request**: (sebagai contoh)

```json
{
    "name": "string",
    "year": "number",
    "author": "string",
    "summary": "string",
    "publisher": "string",
    "pageCount": "number",
    "readPage": "number",
    "reading": "boolean"
}
```

#### Kriteria 7: API dapat menghapus buku

API harus dapat menghapus buku berdasarkan id melalui route:

- **Method**: DELETE
- **URL**: /books/{bookId}



# Dokumentasi API Artikel

## Base Url


## Menambahkan Artikel

Endpoint :/api/artikel

Method : POST 

Headers:

- Content-Type: application/json

Request Body :

```json
{
  "judul" : "Apa itu stunting",
  "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
  "tanggal": "2024-05-14",
  "sumber": "http://sumber.com",
  "gambar": "https://link.gambar.com",
  "kategori": "Semua Kategori"
}
```

Response Body Success :

```json
{
  "message" : "Sukses menambahkan artikel",
  "data" : {
    "id" : 1,
    "judul" : "Apa itu stunting",
    "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
    "tanggal": "2024-05-14",
    "sumber": "http://sumber.com",
    "gambar": "https://link.gambar.com",
    "kategori": "Semua Kategori",
    "createdAt": "2024-05-15 10:51:47",
    "updatedAt": "2024-05-15 10:51:47"
  }
}
```

Response Body Error :

```json
{
  "errors": "Gagal menambahkan artikel"
}
```

## Mengambil Semua data Artikel

Endpoint : /api/artikel

Method : GET

Response Body Success :

```json
{
  "message" : "Sukses mendapatkan data artikel",
  "data": [
    {
      "id" : 1,
      "judul" : "Apa itu stunting",
      "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
      "tanggal": "2024-05-14",
      "sumber": "http://sumber.com",
      "gambar": "https://link.gambar.com",
      "kategori": "Semua Kategori",
    },
    {
      "id" : 2,
      "judul" : "Apa itu stunting",
      "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
      "tanggal": "2024-05-14",
      "sumber": "http://sumber.com",
      "gambar": "https://link.gambar.com",
      "kategori": "6-8 bulan",
    }
  ]
}
```

Response Body Error :

```json
{
  "errors": "Gagal mendapatkan artikel"
}
```

## Mengambil Detail Artikel

Endpoint : /api/artikel/:id

Method : GET

Response Body Success :

```json
{
  "message" : "Sukses mendapatkan detail artikel",
  "data" : {
    "id" : 1,
    "judul" : "Apa itu stunting",
    "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
    "tanggal": "2024-05-14",
    "sumber": "http://sumber.com",
    "gambar": "https://link.gambar.com",
    "kategori": "Semua Kategori",
    "createdAt": "2024-05-15 10:51:47",
    "updatedAt": "2024-05-15 10:51:47"
  }
}
```

Response Body Error :

```json
{
  "errors": "Gagal mendapatkan detail artikel"
}
```

## Mengambil Artikel Berdasarkan Kategori

Endpoint : /api/artikel?kategori=6-8 bulan

Method : GET

Response Body Success :

```json
{
  "message" : "Sukses mendapatkan data artikel",
  "data": [
    {
      "id" : 2,
      "judul" : "Apa itu stunting",
      "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
      "tanggal": "2024-05-14",
      "sumber": "http://sumber.com",
      "gambar": "https://link.gambar.com",
      "kategori": "6-8 bulan",
    }
  ]
}
```

## Pencarian Artikel

Endpoint : /api/artikel?q=Apa

Method : GET

Response Body Success :

```json
{
  "message" : "Sukses mendapatkan data artikel",
  "data": [
    {
      "id" : 2,
      "judul" : "Apa itu stunting",
      "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
      "tanggal": "2024-05-14",
      "sumber": "http://sumber.com",
      "gambar": "https://link.gambar.com",
      "kategori": "6-8 bulan",
    }
    {
      "id" : 3,
      "judul" : "Apa itu penyakit",
      "deskripsi" : "penyakit adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
      "tanggal": "2024-05-14",
      "sumber": "http://sumber.com",
      "gambar": "https://link.gambar.com",
      "kategori": "semua",
    }
  ]
}
```

## Mengubah Data Artikel

Endpoint : /api/artikel/:id

Method : PUT

Headers:

- Content-Type: application/json

Request Body :

```json
{
  "judul" : "Apa itu stunting",
  "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
  "tanggal": "2024-05-14",
  "sumber": "http://sumber.com",
  "gambar": "https://link.gambar.com",
  "kategori": "Semua Kategori"
}
```

Response Body Success :

```json
{
  "message" : "Sukses mengubah artikel",
  "data" : {
    "id" : 1,
    "judul" : "Apa itu stunting",
    "deskripsi" : "Stunting adalah kondisi terhambatnya pertumbuhan fisik dan perkembangan otak pada anak-anak, biasanya disebabkan oleh kurangnya asupan gizi yang memadai dan infeksi pada masa awal kehidupan",
    "tanggal": "2024-05-14",
    "sumber": "http://sumber.com",
    "gambar": "https://link.gambar.com",
    "kategori": "Semua Kategori",
    "createdAt": "2024-05-15 10:51:47",
    "updatedAt": "2024-05-15 10:51:47"
  }
}
```

Response Body Error :

```json
{
  "errors": "Gagal mengubah artikel"
}
```


## Menghapus Data Artikel

Endpoint : /api/artikel/:id

Method : DELETE

Response Body Success :

```json
{
  "data": "Berhasil menghapus artikel"
}
```

Response Body Error :

```json
{
  "errors": "Gagal menghapus artikel"
}
```

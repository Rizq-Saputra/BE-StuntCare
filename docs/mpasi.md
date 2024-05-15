# Dokumentasi API Makanan Pendamping ASI

## Base Url

## Menambahkan Data MPASI

Endpoint : /api/mpasi

Headers:

- Content-Type: application/json

Method : POST

Request Body :

```json
{
  "makanan": "Bubur bayi",
  "porsi": 2,
  "bahan": {
    "kentang": "50gr",
    "telur": "1 butir",
    "kaldu sapi": "50 ml"
  },
  "cara_masak": [
    "Kupas dan potong kentang menjadi potongan kecil-kecil.",
    "Rebus kentang hingga empuk, lalu tiriskan.",
    "Kocok telur dan tambahkan ke dalam kentang yang telah dihaluskan.",
    "Panaskan kaldu sapi dan tambahkan ke dalam campuran kentang dan telur. Aduk hingga merata.",
    "Masak campuran tersebut dengan api kecil hingga mengental dan menjadi bubur yang lembut.",
    "Angkat dan biarkan dingin sebelum disajikan kepada bayi."
  ],
  "kandungan": {
    "kalori": "100 kkal",
    "protein": "6 gr",
    "lemak": "3,5 gr",
    "karbohidrat": "7,8 gr"
  },
  "kategori": "6-8 bulan",
  "gambar": "https://link.gambar.com"
}
```

Response Body Success :

```json
{
  "message": "Sukses menambahkan data Makanan",
  "data": {
    "id": 1,
    "makanan": "Bubur bayi",
    "porsi": 2,
    "bahan": {
      "kentang": "50gr",
      "telur": "1 butir",
      "kaldu sapi": "50 ml"
    },
    "cara_masak": [
      "Kupas dan potong kentang menjadi potongan kecil-kecil.",
      "Rebus kentang hingga empuk, lalu tiriskan.",
      "Kocok telur dan tambahkan ke dalam kentang yang telah dihaluskan.",
      "Panaskan kaldu sapi dan tambahkan ke dalam campuran kentang dan telur. Aduk hingga merata.",
      "Masak campuran tersebut dengan api kecil hingga mengental dan menjadi bubur yang lembut.",
      "Angkat dan biarkan dingin sebelum disajikan kepada bayi."
    ],
    "kandungan": {
      "kalori": "100 kkal",
      "protein": "6 gr",
      "lemak": "3,5 gr",
      "karbohidrat": "7,8 gr"
    },
    "kategori": "6-8 bulan",
    "gambar": "https://link.gambar.com",
    "createdAt": "2024-05-15 10:51:47",
    "updatedAt": "2024-05-15 10:51:47"
  }
}
```

Response Body Error :

```json
{
  "errors": "Gagal menambahkan data Makanan"
}
```

## Mengambil Semua data MPASI

Endpoint : /api/mpasi

Method : GET

Response Body Success :

```json
{
  "message": "Sukses mendapatkan data Makanan",
  "data": [
    {
      "id": 1,
      "makanan": "Bubur bayi",
      "kategori": "6-8 bulan",
      "gambar": "https://link.gambar.com"
    },
    {
      "id": 2,
      "makanan": "alpukat",
      "kategori": "9-11 bulan",
      "gambar": "https://link.gambar.com"
    }
  ]
}
```

Response Body Error :

```json
{
  "errors": "Gagal mendapatkan data Makanan"
}
```

## Mengambil Detail data MPASI

Endpoint : /api/mpasi/:id

Method : GET

Response Body Success :

```json
{
  "message": "Sukses mendapatkan detail Makanan",
  "data": {
    "id": 1,
    "makanan": "Bubur bayi",
    "porsi": 2,
    "bahan": {
      "kentang": "50gr",
      "telur": "1 butir",
      "kaldu sapi": "50 ml"
    },
    "cara_masak": [
      "Kupas dan potong kentang menjadi potongan kecil-kecil.",
      "Rebus kentang hingga empuk, lalu tiriskan.",
      "Kocok telur dan tambahkan ke dalam kentang yang telah dihaluskan.",
      "Panaskan kaldu sapi dan tambahkan ke dalam campuran kentang dan telur. Aduk hingga merata.",
      "Masak campuran tersebut dengan api kecil hingga mengental dan menjadi bubur yang lembut.",
      "Angkat dan biarkan dingin sebelum disajikan kepada bayi."
    ],
    "kandungan": {
      "kalori": "100 kkal",
      "protein": "6 gr",
      "lemak": "3,5 gr",
      "karbohidrat": "7,8 gr"
    },
    "kategori": "6-8 bulan",
    "gambar": "https://link.gambar.com",
    "createdAt": "2024-05-15 10:51:47",
    "updatedAt": "2024-05-15 10:51:47"
  }
}
```

Response Body Error :

```json
{
  "errors": "Gagal mendapatkan detail Makanan"
}
```

## Mengubah Data MPASI

Endpoint : /api/mpasi/:id

Method : PUT

Headers:

- Content-Type: application/json

Request Body :

```json
{
  "makanan": "Bubur",
  "porsi": 2,
  "bahan": {
    "kentang": "50gr",
    "telur": "1 butir",
    "kaldu sapi": "50 ml"
  },
  "cara_masak": [
    "Kupas dan potong kentang menjadi potongan kecil-kecil.",
    "Rebus kentang hingga empuk, lalu tiriskan.",
    "Kocok telur dan tambahkan ke dalam kentang yang telah dihaluskan.",
    "Panaskan kaldu sapi dan tambahkan ke dalam campuran kentang dan telur. Aduk hingga merata.",
    "Masak campuran tersebut dengan api kecil hingga mengental dan menjadi bubur yang lembut.",
    "Angkat dan biarkan dingin sebelum disajikan kepada bayi."
  ],
  "kandungan": {
    "kalori": "100 kkal",
    "protein": "6 gr",
    "lemak": "3,5 gr",
    "karbohidrat": "7,8 gr"
  },
  "kategori": "6-8 bulan",
  "gambar": "https://link.gambar.com",
}
```

Response Body Success :

```json
{
  "message": "Sukses mengubah data Makanan",
  "data": {
    "id": 1,
    "makanan": "Bubur",
    "porsi": 2,
    "bahan": {
      "kentang": "50gr",
      "telur": "1 butir",
      "kaldu sapi": "50 ml"
    },
    "cara_masak": [
      "Kupas dan potong kentang menjadi potongan kecil-kecil.",
      "Rebus kentang hingga empuk, lalu tiriskan.",
      "Kocok telur dan tambahkan ke dalam kentang yang telah dihaluskan.",
      "Panaskan kaldu sapi dan tambahkan ke dalam campuran kentang dan telur. Aduk hingga merata.",
      "Masak campuran tersebut dengan api kecil hingga mengental dan menjadi bubur yang lembut.",
      "Angkat dan biarkan dingin sebelum disajikan kepada bayi."
    ],
    "kandungan": {
      "kalori": "100 kkal",
      "protein": "6 gr",
      "lemak": "3,5 gr",
      "karbohidrat": "7,8 gr"
    },
    "kategori": "6-8 bulan",
    "gambar": "https://link.gambar.com",
    "createdAt": "2024-05-15 10:51:47",
    "updatedAt": "2024-05-15 11:48:39"
  }
}
```

Response Body Error :

```json
{
  "errors": "Gagal mengubah data Makanan"
}
```

## Menghapus Data MPASI

Endpoint : /api/mpasi/:id

Method : DELETE

Response Body Success :

```json
{
  "data": "Berhasil menghapus data makanan"
}
```

Response Body Error :

```json
{
  "errors": "Gagal menghapus data makanan"
}
```

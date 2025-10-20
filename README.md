# Cilame_GeoJson

## Dokumentasi Data Geospasial
Data ini berisi jalur jalan (LineString) yang telah diubah dari format GeoJSON FeatureCollection menjadi array dokumen JSON individual, siap untuk di-insert ke MongoDB.

## Peta Digital Jalan Wilayah Cilame 🗺️
Repositori ini berisi data geospasial (peta) dari beberapa ruas jalan penting di Wilayah Cilame. Seluruh data disajikan dalam format GeoJSON yang modern dan mudah diintegrasikan dengan berbagai platform, dioptimalkan untuk basis data MongoDB.

## 📌 Data Jalan yang Tersedia
Berikut adalah daftar 6 ruas jalan yang datanya tersedia dalam repositori ini, berdasarkan pemisahan dari data GeoJSON awal:

1. JL. Muhajirin

2. JL. Bukit Indah

3. JL. Bukit Indah 1

4. JL. Bukit Indah 4

5. JL. Graha Bukit Raya 3

6. JL. Ganesha IV

## Format Data & Struktur MongoDB
Setiap objek dalam array merepresentasikan satu dokumen di koleksi Anda dan mengikuti standar GeoJSON untuk kolom geometry.

```
{
  "name": "Nama Lokasi/Jalan",
  "geometry": {
    "type": "LineString", // atau "Point", "Polygon"
    "coordinates": [
      // array koordinat [longitude, latitude]
    ]
  }
}
```